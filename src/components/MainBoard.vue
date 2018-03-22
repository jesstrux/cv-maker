<style scoped>
  #mainBoard{
    background: #00f;
  }
  #theBoard{
    background: #f8f8f8;
    flex: 1;
    display: grid;
    grid-gap: 0em;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(5, 1fr);
  }

  #theBoard > div{
    color: #fff;
    padding: 1.4em;
    position: relative;
    overflow: hidden;
  }

  #theBoard > div .preview, 
  #theBoard > div:after{
    content: '';
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    z-index: 0;
  }

  #theBoard > div .preview{
    transition: all 0.25s ease-out;
    background-color: #ddd;
    background-size: cover;
    background-position: center;
  }

  #theBoard > div h3{
    position: relative;
    z-index: 1;
  }

  #theBoard > div button{
    padding: 0.2em 0.5em;
    position: absolute;
    bottom: 1em;
    right: 1em;
    border: 2px solid #eee;
    background: transparent;
    z-index: 1;
  }

  #theBoard > div button svg{
    width: 1.8em;
    height: 1.8em;
    fill: #eee;
  }

  #theBoard > div:hover .preview{
    transform: scale(1.3);
  }
  
  #theBoard > div:after{
    background: #000;
    opacity: 0.3;
  }

  #music{
    grid-area: 1/3/4/5;
  }

  #music .preview{
    background-image: url('../assets/images/album3.jpg');
  }

  #youtube{
    grid-area: 1/1/3/3;
  }

  #youtube .preview{
    background-image: url('../assets/images/yt4.jpg');
  }

  #images{
    grid-area: 3/1/6/3;
  }

  #images .preview{
    background-image: url('../assets/images/img2.jpg');
  }

  #articles{
    grid-area: 4/3/6/5;
  }

  #articles .preview{
    background-image: url('../assets/images/articles.png');
  }
</style>


<template>
  <div id="mainBoard">
    <div class="section-title">
      <h1>OFFICE BOARD</h1>
    </div>
    <div id="theBoard">
      <div id="images">
        <h3>IMAGES&nbsp; &amp; &nbsp;VIDEOS</h3>
        <div class="preview"></div>
        <button>
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
        </button>
      </div>
      <div id="music">
        <h3>MUSIC PLAYLIST</h3>
        <div class="preview"></div>
        <button>
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
        </button>
      </div>
      <div id="youtube">
        <h3>YOUTUBE VIDEOS</h3>
        <div class="preview"></div>
        <button>
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
        </button>
      </div>
      <div id="articles">
        <h3>ARTICLES&nbsp; &amp; &nbsp;LINKS</h3>
        <div class="preview"></div>
        <button>
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'MainBoard',
    components: { },
  }
</script>