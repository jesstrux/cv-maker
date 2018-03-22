<template>
  <div id="onlineUsers">
    <div class="section-title">
      <h1>DIRECT CHAT</h1>
    </div>
    <div id="chatArea" class="flex">
      
    </div>
    <div id="input" class="layout center justified">
      <input class="flex" type="text" placeholder="Type to write your message.">
      <button>
        <svg fill="#fff" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M2.01 21L23 12 2.01 3 2 10l15 2-15 2z"/></svg>
      </button>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'OnlineUsers',
    components: { },
  }
</script>

<style scoped>
  #chatArea{
    overflow: auto;
    padding: 1.4em;
  }
  #input{
    position: relative;
    width: 100%;
    background: #fff;
    height: 55px;
    box-shadow: 0 -2px 0 rgba(0, 0, 0, 0.03)
  }

  #input input{
    /* position: absolute; */
    /* left: 0; */
    /* top: 0; */
    /* width: 100%; */
    height: 100%;
    flex: 1;
    border: none;
    outline: 0;
    background: transparent;
    font-size: 1.1em;
    padding: 0 0.9em;
  }

  #input button{
    margin: 0 0.5em;
    padding: 0.5em 0.8em;
    background: black;
    border: none;
    color: #fff;
  }
</style>