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
        <div class="m"><button>check</button></div>
      </div>

      <div class="box2">
        <div class="n"><input v-for="i in 28" :key="i" type="checkbox" /></div>
      </div>

      <div class="box3">
        <div class="o">Time:</div>
        <div class="p">not yet set</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

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
  background: red;
  padding: 70px;
}

.box2 {
  background: blue;
  padding-right: 100px;
  padding-left: 100px;
  border-left: solid;
  border-bottom: solid;
}

.box3 {
  background: green;
  display: flex;
}

.a{
  font-size: 15px;
  font-weight: 600;
  letter-spacing:0px;
  margin-top:20px;
  margin-left: 15px;
}

.b{
  font-size: 12px;
  font-weight: bold;
  letter-spacing: -0.5px;
  /* margin-left: 470px;
  margin-top: 300px; */
}

.c{
  font-size: 13px;
  font-weight: 100;
  /* margin-left: 470px; */
  margin-top: 10px;
}

.i{
  margin-top: 10px;
}

.j{
  font-size: 13px;
  /* margin-left: 470px; */
  }

.k{
  margin-top: 20px;
}

.l{
  margin-top: -3px;
}

.m{
  margin-top: 15px;
  /* margin-left: 470px; */
}

.n{
  padding-top: 200px;
}

.o{
  padding-left: 30px;
  font-size: 11px;
  font-weight: bold;
}

.p{
  font-size: 11px;

}
</style>