<template>
  <div id="app">
    <div class="section1">
      <div class="header">
        {{ header }}
      </div>
      <div class="subheader">
        <h3>{{ subheader }}</h3>
      </div>
    </div>
    <div class="section2">
      <div class="content">
        <div class="row">
          <div class="col-md-6">
            <h2 class="title">{{ section2.headline }}</h2>
            <!--<p>{{ section2.paragraph }}</p>-->
          </div>
          <div class="col-md-6">
            <img :src="section2.image1Path"/>  
            <p>{{ section2.paragraph2 }}</p>
          </div>
        </div>
      </div>  
    </div>
    <div class="section3">
      
    </div>
    <div class="section4">
      
    </div>
    <div class="section5">
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      header: 'CaçambotW200',
      subheader: 'Ao fim do dia, todos se tornam entulho...',
      section2: {
        headline: "",
        paragraph: "me mata memata metamamra mem mata maemtame metmea me mete me mata. Mme mata memata metamamra mem mata maemtame metmea me mete me mata.",
        paragraph2: "succ ma thicc dick succ ma thicc succ ma thicc succ ma thicc succ ma thicc succ ma thicc dick",
        image1Path: "/src/assets/img/cacambot.png"
      }
    }
  }
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css?family=Raleway:800');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
  height: 100%;
  width: 100%;
  font-family: 'Raleway';
}

html, body { 
    margin: 0; 
    padding: 0; 
    width: 100%; 
    height: 100%;
}

h1, h2 {
  font-weight: normal;
  margin: 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.section1 {
  background: url('assets/img/s-1.png') no-repeat 50% 0%;
  height: 900px;
}
.section2 {
  background: url('assets/img/s-2.png') no-repeat 0%;
  height: 900px;
}

.header {
  font-size: 4em;
  position: absolute;
  top: 15%;
  left: 5%;
}
.subheader {
  font-size: 2em;
  position: absolute;
  top: 25%;
  left: 40%;
  background-color: rgba(0,0,0,0.2);
  box-sizing: border-box;
  padding: 0 5%;
}
.content {
  color: white;
  padding: 0;
}
.title {
  text-align: center;
  font-family: 'Oswald', Helvetica, sans-serif;
  font-size: 80px;
  transform: skewY(-10deg);
  letter-spacing: 4px;
  word-spacing: -8px;
  color: #728a37;
  text-shadow: 
    -1px -1px 0 #aac46b,
    -2px -2px 0 #aac46b,
    -3px -3px 0 #aac46b,
    -4px -4px 0 #aac46b,
    -5px -5px 0 #aac46b,
    -6px -6px 0 #aac46b,
    -7px -7px 0 #aac46b,
    -8px -8px 0 #aac46b,
    -30px 20px 40px dimgrey
}
</style>
