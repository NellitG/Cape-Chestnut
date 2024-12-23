<template>
    <div class="mt-10">
      <h1>Real-Time Chat</h1>
      <!-- <div class="">
        <div v-for="(msg, index) in messages" :key="index" class="chat-message">
          {{ msg }}
        </div>
      </div> -->
      <input
        type="text"
        v-model="message"
        @keyup.enter="sendMessage"
        placeholder="Type a message"
      />
      <button @click="sendMessage">Send</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        socket: null,
        messages: [],
        message: "",
      };
    },
    methods: {
      connectWebSocket() {
        const wsUrl = `${window.location.protocol === "https:" ? "wss" : "ws"}://${
          window.location.host
        }/ws/chat`;
  
        this.socket = new WebSocket(wsUrl);
  
        this.socket.onmessage = (event) => {
          this.messages.push(event.data);
        };
  
        this.socket.onopen = () => {
          console.log("Connected to WebSocket server.");
        };
  
        this.socket.onclose = () => {
          console.log("Disconnected from WebSocket server.");
        };
  
        this.socket.onerror = (error) => {
          console.error("WebSocket error:", error);
        };
      },
      sendMessage() {
        if (this.message.trim() !== "") {
          this.socket.send(this.message);
          this.message = "";
        }
      },
    },
    mounted() {
      this.connectWebSocket();
    },
    beforeDestroy() {
      if (this.socket) {
        this.socket.close();
      }
    },
  };
  </script>
  
  <style scoped>
  .chat-app {
    max-width: 500px;
    margin: auto;
    font-family: Arial, sans-serif;
  }
  
  .chat-window {
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 10px;
    height: 300px;
    overflow-y: auto;
    margin-bottom: 10px;
  }
  
  .chat-message {
    background: #f1f1f1;
    padding: 5px 10px;
    margin-bottom: 5px;
    border-radius: 3px;
  }
  
  input {
    width: calc(100% - 60px);
    padding: 10px;
    margin-right: 5px;
  }
  
  button {
    padding: 10px;
  }
  </style>
  