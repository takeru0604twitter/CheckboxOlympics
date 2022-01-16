<template>
  <div>
    <div class="a">CheckB<input type="checkbox" checked class="a1">x <input type="checkbox" checked calss="a2">lympics</div>
    
    <div class="box">
      <div class="box1">
        <div class="b">100 Meter Sprint</div>
        <div class="c">
          <div class="d">When the start</div>
          <div class="e">board reads Go,</div>
          <div class="f">begin clicking,</div>
          <div class="g">speed is what</div>
          <div class="h">matters here.</div>
          <div class="i">Don't false start.</div>
        </div>
        <div class="j">
          <div class="k"><a href="https://checkboxolympics.com/#:~:text=Watch%20how%20on%20YouTube">Watch how on </a></div>
          <div class="l"><a href="https://checkboxolympics.com/#:~:text=Watch%20how%20on%20YouTube">Youtube</a></div>
        </div>
        <div class="m">
          <button @click="ready">ready</button>
        </div>
      </div>

      <div class="box2">
        <div class="t">
          <div class="q">SET</div>
          <div class="r">/</div>
          <div class="s">GO</div>
        </div>
          <div class="n"><input v-for="i in 28" :key="i" type="checkbox" /></div>
      </div>

      <div class="box3">
        <div @click="Time" class="o">Time:&nbsp;</div>
        <!-- <div class="p">not yet set</div> -->
        <div class="p">{{ time }}</div>
      </div> 
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      time: undefined,
      a: undefined,
      b: 0
    }
  },
  methods: {
    ready() { 
      console.log('check button is pushed')
      const setButton = document.getElementsByClassName('q')[0]

      setButton.style.backgroundColor = 'orange'

      setTimeout('console.log(s)',3);
    
      const GOButton =document.getElementsByClassName('s')[0]

      GOButton.style.backgroundColor = 'green'
    },
    Time() {
      const date = new Date()
      this.time = date
    }
  }
}
</script>

<style>
body {
  margin: 0px;
}

.box {
  position: relative;
  display: flex;
  margin-top:  250px;
  margin-left: 400px;
}

.box1 {
  padding: 70px;
}

.box2 {
  padding-right: 100px;
  padding-left: 100px;
  border-left: solid;
  border-bottom: solid;
}

.box3 {
  display: flex;
}

.a{
  font-size: 16px;
  font-weight: 600;
  letter-spacing:-1px;
  margin-top:20px;
  margin-left: 20px;
}

.a1{
  width: 9px;
  height: 9px;
}

.a2{
  width: 10px;
  height: 10px;
}

.b{
  font-size: 12px;
  font-weight: bold;
  letter-spacing: -0.5px;
}

.c{
  font-size: 13px;
  font-weight: 100;
  margin-top: 10px;
}

.i{
  margin-top: 10px;
}

.j{
  font-size: 13px;
  }

.k{
  margin-top: 20px;
}

.l{
  margin-top: -3px;
}

.m{
  margin-top: 15px;
}

.n{
  padding-top: 150px;
}

.o{
  padding-left: 30px;
  font-size: 11px;
  font-weight: bold;
}

.p{
  font-size: 11px;

}

.q{
  color: white;
  background-color:gray;
}

.s{
  color: white;
  background-color:gray;
}

.t{
  display: flex;
  padding-top: 20px;
}
</style>