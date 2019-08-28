<template>
  <body>
    <header>
      <nav id="navbar">
        <ul style="list-style: none;">
          <li><a href="#about">About Me</a></li>
          <li><a href="#work">Past Work</a></li>
          <li><a href="#contact">Contact Me</a></li>
        </ul>
      </nav>

      <h1 id="name">Maren Luper</h1>
    </header>

    <!--<div class="container">
    </div>-->

    <section id="welcome-section">
      <h1 id="welcome">Web Developer, UX/UI Design</h1>
      <div class="container" id="bio-box">
        <div class="container" id="bio-grid">
          <p id="bio">Current Integrated Science and Technology student at James Madison University, concentrating in information systems, experience with website development and team-oriented front-to-back application development.</p>
          <ul style="list-style: none;">
            <li>Java, JavaScript, Python</li>
            <li>Certified in Responsive Web Design (HTML5/CSS)</li>
          </ul>
        </div>

        <a href="https://ibb.co/dhso0p"><img src="https://image.ibb.co/nqhAD9/IMG_1663.jpg" alt="IMG_1663" border="0" id="biopic1"></a>
      </div>
    </section>

    <section id="projects">
      <h1 id="work">My Past Work</h1>
      <p id="profile">To see where I earned my credentials, visit my <a href="https://www.freecodecamp.org/maren_521" target="_blank" id="profile-link">FCC profile</a></p>
      <div id="arrow-left">
      </div>
      <div id="arrow-right">
      </div>
      <div class="container" id="tiles-box">
        <div class="list" id="tiles">
          <div class="project-tile">
            <a href="https://codepen.io/maren521/full/qrwzwM/"><img src="https://preview.ibb.co/jDvSrU/2018_08_10_18_42_28.png" alt="2018_08_10_18_42_28" border="0" id="1"></a>
          </div>
          <div class="project-tile">
            <a href="https://codepen.io/maren521/full/bqzmVz/"><img src="https://preview.ibb.co/g7y2Qp/2018_08_10_18_43_16.png" alt="2018_08_10_18_43_16" border="0" id="2"></a>
          </div>
          <div class="project-tile">
            <a href="https://codepen.io/maren521/full/djqRvR/"><img src="https://preview.ibb.co/i560BU/2018_08_10_18_44_13.png" alt="2018_08_10_18_44_13" border="0" id="3"></a>
          </div>
          <div class="project-tile">
            <a href="https://codepen.io/maren521/pen/OwBKKJ"><img src="https://preview.ibb.co/hpifBU/2018_08_10_18_45_18_Window.png" alt="2018_08_10_18_45_18_Window" border="0" id="4"></a>
          </div>
        </div>
      </div>
    </section>

    <section id="contacts">
    </section>

  </body>
</template>

<script>
export default {
  data () {
    return {
      title: 'Portfolio'
    }
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css?family=Buda:300|Cherry+Swash|Courgette|Delius|Flamenco|Lancelot|Merienda|Overlock+SC|Poiret+One|Sacramento|Sail|Tangerine|Unica+One');

  header {
    position: fixed;
    display: flex;
    width: 100%;
    align-items: center;
    justify-content: space-between;
    top: 0;
    margin-left: -10px;
    padding-left: 10px;
    background-color: hsl(100, 50%, 60%)
  }

  @media (max-width: 700px) {
    header {
      flex-wrap: wrap;
    }
  }

  #name {
    font-size: 40px;
    font-family: Cherry Swash;
    padding-left: 28px;
  }

  nav {
    display: flex;
    position: fixed;
    top: 0;

    ul {
      display: flex;
      flex-direction: row;
      margin: 10px 0px 5px 420px;
      justify-content: flex-end;
      align-items: center;
      text-align: center;
      font-family: Cherry Swash, Columbia;
      font-size: 20px;
      width: 58vw;
    }

    li {
      padding: 30px 20px 0px 100px;
      margin-bottom: 0px;
      margin-top: 0px;
    }
  }

  a {
    text-decoration: none;
    color: black;
    &:hover {
      color: #ddd;
    }
  }

  p {
    text-align: center;
  }

  #profile-link {
    color: orange;
    &:hover {
      color: #ddd;
    }
  }

  /**Welcome Section*/
  #welcome {
    font-size: 62px;
    font-family: Buda;
    margin-top: 100px;
    margin-left: 20px;
  }

  #welcome-section {
    display: block;
    height: 100vh;
    margin-bottom: 0px;
  }

  #bio-box {
    display: grid;
    grid-template-columns: 1fr 1fr;
    justify-items: center;
    align-items: space-around;

    #bio-grid {
      display: grid;
      grid-template-rows: 40% 60%;
      justify-items: center;
      width: 500px;
      margin: 0px 140px 0px 100px;
      font-size: 20px;
      font-family: Buda;

      ul {
        width: 500px;
        text-align: center;
      }
    }

    #biopic1 {
      width: 280px;
      height: auto;
      margin: -60px 30px 30px 0px;
    }
  }

  /**Projects Section*/
  #projects {
    padding-top: 120px;
    margin-top: 0px;
  }

  #work {
    text-align: center;
    font-size: 62px;
    font-family: Buda;
  }

  #profile {
    font-size: 20px;
    font-family: Buda;
  }

  img {
    height: 100%;
    width: 100%;
  }

  .project-tile {
    background-color: blue;
    position: relative;
    width: 300px;
    height: 150px;
    margin: 5px 10px 5px 10px;
  }

  #tiles-box {
    display: flex;
    justify-content: center;
    #tiles {
      display: flex;
      align-items: center;
      margin-top: 50px;
    }
  }
</style>
