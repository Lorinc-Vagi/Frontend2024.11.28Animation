<script>
  // div golyóm
  var gonoszRad =100

  var x=0 
  var y=0
  var xi=4
  var yi=4
  setInterval(() => {
    x += xi
    y += yi
    yi+=0.01
    // xi*=0.999
    // yi*=0.999
    if (x >= window.innerWidth-gonoszRad || x<=0) {
      xi *= -1
    }
    if (y >= window.innerHeight-gonoszRad || y<=0) {
      yi *= -1
    }
  })

  



    // div golyóm
  var staticRad1 =100

  var x1=500  //window.innerWidth-staticRad1-5
  var y1=500//window.innerHeight-staticRad1-5
  var xi1=-0
  var yi1=-0
  setInterval(() => {
    // x1 += xi1
    // y1 += yi1
    // yi1+=0.01
    // xi*=0.999
    // yi*=0.999
    // if (x1 >= window.innerWidth-staticRad1 || x1<=0) {
    //   xi1 *= -1
    // }
    // if (y1 >= window.innerHeight-staticRad1 || y1<=0) {
    //   yi1 *= -1
    // }
  }
  )
</script>

<main>
  <!-- <input type="text" name="" id="" bind:value={x}>
  <input type="text" name="" id="" bind:value={y}> -->
  <div class="golyorosz golyo" style="left: {x}px; top: {y}px; width: {gonoszRad}px; height: {gonoszRad}px;" >
    <p style="font-size: 20px;">>:(</p>
  </div>
  <div class="golyo1 golyo" style="left: {x1}px; top: {y1}px; width: {staticRad1}px; height: {staticRad1}px;" >
  </div>
  <div class="text">
    <!-- <p>y: {y}</p>
    <p>x: {x}</p> -->
  </div>
</main>

<style>

  .text{
    left:0px;
    top:0px;
  }
  .golyo{
    position: fixed;
  }

  .golyorosz{
    background-color: red;
    border-radius: 100%;
  }
  .golyo1{
    background-color: green;
    border-radius: 100%;
  }
</style>
