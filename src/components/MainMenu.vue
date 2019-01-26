<template>
  <div>
    <div class="grid-container">
      <div class="grid-item">
        <img class="poster" src="poster_test.jpg">
        <div class="overlay">
          <div class="text">Avenger : End Game</div>
        </div>
      </div>
      <div class="grid-item">
        <img class="poster" src="poster_test.jpg">
        <div class="overlay">
          <div class="text">Hello World</div>
        </div>
      </div>
      <div class="grid-item">
        <img class="poster" src="poster_test.jpg">
        <div class="overlay">
          <div class="text">Hello World</div>
        </div>
      </div>
      <div class="grid-item">
        <img class="poster" src="poster_test.jpg">
        <div class="overlay">
          <div class="text">Hello World</div>
        </div>
      </div>
      <div class="grid-item">
        <img class="poster" src="poster_test.jpg">
        <div class="overlay">
          <div class="text">Hello World</div>
        </div>
      </div>
      <div class="grid-item">
        <img class="poster" src="poster_test.jpg">
        <div class="overlay">
          <div class="text">Hello World</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
/* home card movie */

.grid-container {
  width: 1000px;
  display: grid;
  margin: auto;
  margin-top: 100px;
  grid-template-columns: auto auto auto auto;
}

.grid-item {
  position: relative;
  background-color: rgba(255, 255, 255, 0.8);
  margin: 0 0px 32px 0;
  width: 225px;
  height: 350px;
  padding: 0px;
  font-size: 30px;
  text-align: center;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgb(255, 255, 255);
  overflow: hidden;
  width: 100%;
  height: 20%;
  transition: 0.5s ease;
}

.grid-item:hover .overlay {
  height: 100%;
}
.poster {
  width: 100%;
  height: 80%;
}
.text {
  font-size: 22px;
  padding: 2px;
}
</style>


