<script>
</script>

<body>
<section class="container">
  <div class="text">C</div>
  <span>Coding... </span>
  <div class="moving-background"></div>
</section>
</body>

<style>

body {
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  position: relative;
  display: inline-block;
}

.text {
  font-size: 5em;
  font-weight: bold;
  background: linear-gradient(50deg, #ff0, #00f);
  display: inline-block;
  padding: 10px;
  animation: scaleColorChange 1s infinite alternate;
  -webkit-background-clip: text;
  background-clip: text;
  text-shadow: 0 0 3px rgb(255, 255, 255), 4px 10px 0 #000000;
  opacity: 1;
}

/* Typewriting -effect */

span{
  letter-spacing: 10px;
  border-right: 2px solid #ff0;
  width: 100%;
  white-space: nowrap;
  overflow: hidden;
  animation:
    typing 2s,
    cursor .4s step-end infinite alternate;
}


@keyframes cursor {
  50% { border-color: transparent }
}

@keyframes typing { from { width: 0 } }

/* Textscale -Animation */

@keyframes scaleColorChange {
  0% {
    transform: scale(1);
    color: #ff4500;
  }
  50% {
    transform: scale(6);
    color: rgb(44, 188, 70);
  }
}

/* Background color */

.moving-background {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background: linear-gradient(50deg, #ff0, #00f); 
  z-index: -1;
}

</style>
