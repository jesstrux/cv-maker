<template>
  <div id="app">
    <div id="cvWrapper" class="layout vertical">
      <div id="title" class="layout vertical center-center">
        <h2 id="name">
          Walter Kimaro
        </h2>
        <p id="profession">
          Web Developer
        </p>
      </div>
      <div id="mainContent" class="layout flex">
        <div id="miniSections">
          <div id="contacts" class="mini-section">
            <h3>CONTACTS</h3>
            <div class="layout center end-justified">
              <span>+255 717 138 056</span>
            </div>
            <div class="layout center end-justified">
              <span>wakyj07@gmail.com</span>
            </div>
            
            <div class="layout center end-justified">
              <span>linkedin.com/in/wkimaro</span>
            </div>
          </div>
          <div id="education" class="mini-section">
            <div class="item">
              <h3>EDUCATION</h3>
              <h5>Tanga Technical</h5>
              <p>Tanga - Tanga</p>
            </div>
            
            <div class="item">
              <h5>Moshi Technical</h5>
              <p>Moshi - Kilimanjaro</p>
            </div>
          </div>
          <div id="skills" class="mini-section">
            <h3>SKILLS</h3>
            <p>HTML & CSS</p>
            <p>Javascript</p>
            <p>PHP</p>
            <p>Laravel</p>
            <p>Jquery + (UI & Mobile)</p>
            <p>Angular, AngularJS</p>
            <p>Vuejs</p>
            <p>Polymer</p>
            <p>Ionic</p>
            <p>Phonegap, Cordova</p>
            <p>Git & Github</p>
          </div>
        </div>
        <div id="divider"></div>
        <div id="longSections" class="flex">
          <div id="about">
            <p>
              I am a detail oriented web developer who offers immense attention to detail for
              both desktop and mobile web solutions. I am passionate about creating web experiences
              that are rooted in not only beautiful and catchy user interfaces but also easy to use 
              and straightforward user experiences with special focus on the required business value.
            </p>
          </div>
          
          <div id="experience">
            <h3>EXPERIENCE</h3>
            <div class="section-item">
              <h5>IPF Softwares | June 2017 - Present</h5>
              <h5>Web Developer & Designer</h5>
            </div>
            
            <div class="section-item">
              <h5>Soma Apps | Oct 2016 - June 2017</h5>
              <h5>Web Developer</h5>
            </div>
            
            <div class="section-item">
              <h5>SoftMed | Feb 2016 - Jul 2016</h5>
              <h5>Consultant</h5>
            </div>
          </div>

          <div id="works">
            <h3>FEATURED WORK</h3>
            <div class="section-item">
              <h5>Buni Divaz(http://bunidivaz.co.tz/)</h5>
              <h5>Web Developer</h5>
            </div>

            <div class="section-item">
              <h5>Biashara Plus (http://jesstrux.github.io/bpluslandingpage)</h5>
              <h5>Web Developer</h5>
            </div>

            <div class="section-item">
              <h5>Impact Advisory (http://impactadvisory.co.tz/)</h5>
              <h5>Web Developer</h5>
            </div>

            <div class="section-item">
              <h5>Jua Katiba(http://juakatibatanzania.com/)</h5>
              <h5>Frontend Developer</h5>
            </div>

            <div class="section-item">
              <h5>KidCity(http://kidcity.co.tz/)</h5>
              <h5>Frontend Developer</h5>
            </div>

            <div class="section-item">
              <h5>MisosiHub(https://misosihub.com)</h5>
              <h5>Project Manager, UI/UX Consultant</h5>
            </div>

            <div class="section-item">
              <h5>Olbongo(https://www.olbongo.com)</h5>
              <h5>Frontend Developer, UI/UX Consultant</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import MusicPlaylist from '@/components/MusicPlaylist'
  import MainBoard from '@/components/MainBoard'
  import OnlineUsers from '@/components/OnlineUsers'

  export default {
    name: 'App',
    components: { MusicPlaylist, MainBoard, OnlineUsers },
  }
</script>
	
<style>
  #app{
    overflow: auto;
    height: 100vh;
    background: #f0f0f0;
  }

  #cvWrapper{
    position: relative;
    background: #fff;
    /* width: 595px; */
    /* height: 842px; */
    width: 794px;
    height: 1123px;
    padding: 1% 2%;
    margin: 2em auto;
    overflow: hidden;
    box-shadow: 1px 1px 4px rgba(0, 0, 0, 0.3);
  }

  #title{
      padding-top: 5em;   
      padding-bottom: 1.5em;  
      text-align: center;
      text-transform: uppercase;
      margin-left: 2em;
      margin-right: 2em;  
      margin-bottom: 1.5em;
      border-bottom: 2px solid #75e8e3;
      flex-shrink: 0;
  }

  #name{
      font-family: Bold;
      font-size: 2.2em;
      margin-bottom: 0.3em;
  }

  #profession{
      font-family: Light;
      font-size: 1.2em;
  }

  #mainContent{
      margin-bottom: 0.8em;
  }

  #miniSections{
      width: 30%;
      /*width: 230px;*/
      /*padding-right: 1em;*/
      /*margin-right: 1em;*/
      /*border-right: 1px solid #999;*/
  }

  #divider{
      margin: 0 1.5em;
      width: 0;
      border-right: 1px solid #ccc;
  }

  .mini-section{
      padding-top: 1em;
      text-align: right;
  }

  .mini-section:first-child{
      padding-top: 0.8em;
  }

  h3{
      color: #932727;
      font-weight: 500;
      /*font-family: Bold;*/
      font-size: 1em;
      margin-bottom: 0.4em;
  }

  .mini-section h5, 
  .mini-section p{
      font-size: 0.9em;
      line-height: 1.5em;
      color: #777;
  }

  .mini-section h5{
      /* font-family: SemiBold; */
      color: #000;
  }

  .mini-section h5 + p{
      margin-top: -0.2em;
  }

  #contacts > .layout{
      padding: 0.2em 0;
  }

  #contacts > .layout > span{
      font-size: 0.9em;
  }

  #contacts i{
      margin-left: 0.5em;
      width: 20px;
      height: 20px;
      background: #777;
      border-radius: 50%;
      flex-shrink: 0;
  }

  #contacts svg{
      fill: #fff;
      width: 12px;
      height: 12px;
  }

  #education > .item,
  .section-item{
      margin-bottom: 0.4em;
  }

  h5, p{
      font-size: 0.9em;
      line-height: 1.5em;
      color: #777;
  }

  h5{
      font-size: 1.01em;
      color: #000;
  }

  h5 + h5{
      font-size: 0.95em;
      color: #555;
      margin-top: -0.2em;
  }

  #about{
      margin-top: 0.5em;
      margin-bottom: 1em;
  }

  #experience{
      margin-bottom: 1.2em;
  }

  @media print{
    @page {
      size: A4 portrait;
        margin: 0;
    }
    
    #cvWrapper{
        width: 100vw;
        height: 100vh;
        padding: 1% 4%;
        box-shadow: none;
        margin: 0;
        overflow: visible;
    }
    
    #app{
      overflow: visible;
      height: auto;
      background: transparent;
    }

    #contacts i{
      display: none;
    }

    #divider{
      margin: 0 1.5em;
    }
  }
</style>