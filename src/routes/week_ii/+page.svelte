<script>
  import Title from "$lib/componenten/Title.svelte";

</script>

<main>
  <Title /> 
  <div class="svg-container">
    <svg width="200" height="500" viewBox="-100 -200 200 400">
      <polygon points="0,0 80,120 -80,120" fill="#234236" />
      <polygon points="0,-40 60,60 -60,60" fill="#0C5C4C" />
      <polygon points="0,-80 40,0 -40,0" fill="#38755B" />
      <rect x="-20" y="120" width="40" height="30" fill="brown" />
    </svg>
    </div>

  <ul class="circles">
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
  </ul>
</main>

<style>
.svg-container {
      float: right; /* Plaats de container aan de rechterkant */
      margin-right: 20px; /* Voeg wat marge toe aan de rechterkant (aanpassen indien nodig) */
    }

  /* ANIMATED BACKGROUND */
  .circles {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    overflow: hidden;
    z-index: 0; 

  }

  .circles li {
    position: absolute;
    display: block;
    list-style: none;
    width: 20px;
    height: 20px;
    background-color: var(--background-colo);
    background-image: linear-gradient(225deg, #4e7141 50%, #ff8d06 130%);
    animation: animate 25s linear infinite;
    bottom: -150px;
  }

  .circles li:nth-child(1) {
    left: 25%;
    width: 80px;
    height: 80px;
    animation-delay: 0s;
  }

  .circles li:nth-child(2) {
    left: 10%;
    width: 20px;
    height: 20px;
    animation-delay: 2s;
    animation-duration: 12s;
  }

  .circles li:nth-child(3) {
    left: 70%;
    width: 20px;
    height: 20px;
    animation-delay: 4s;
  }

  .circles li:nth-child(4) {
    left: 40%;
    width: 60px;
    height: 60px;
    animation-delay: 0s;
    animation-duration: 18s;
  }

  .circles li:nth-child(5) {
    left: 65%;
    width: 20px;
    height: 20px;
    animation-delay: 0s;
  }

  .circles li:nth-child(6) {
    left: 75%;
    width: 110px;
    height: 110px;
    animation-delay: 3s;
  }

  .circles li:nth-child(7) {
    left: 35%;
    width: 150px;
    height: 150px;
    animation-delay: 7s;
  }

  .circles li:nth-child(8) {
    left: 50%;
    width: 25px;
    height: 25px;
    animation-delay: 15s;
    animation-duration: 45s;
  }

  .circles li:nth-child(9) {
    left: 20%;
    width: 35px;
    height: 35px;
    animation-delay: 2s;
    animation-duration: 35s;
  }

  .circles li:nth-child(10) {
    left: 85%;
    width: 150px;
    height: 150px;
    animation-delay: 0s;
    animation-duration: 11s;
  }

  .circles li:nth-child(11) {
    left: 5%;
    width: 60px;
    height: 60px;
    animation-delay: 0s;
    animation-duration: 11s;
  }

  .circles li:nth-child(12) {
    left: 55%;
    width: 67px;
    height: 67px;
    animation-delay: 2s;
    animation-duration: 3s;
  }

  .circles li:nth-child(13) {
    left: 15%;
    width: 40px;
    height: 40px;
    animation-delay: 2s;
    animation-duration: 20s;
  }

  .circles li:nth-child(14) {
    left: 80%;
    width: 30px;
    height: 30px;
    animation-delay: 5s;
  }

  .circles li:nth-child(15) {
    left: 45%;
    width: 90px;
    height: 90px;
    animation-delay: 8s;
    animation-duration: 25s;
  }

  .circles li:nth-child(16) {
    left: 60%;
    width: 50px;
    height: 50px;
    animation-delay: 3s;
  }

  .circles li:nth-child(17) {
    left: 25%;
    width: 120px;
    height: 120px;
    animation-delay: 1s;
    animation-duration: 30s;
  }

  .circles li:nth-child(13) {
    left: 15%;
    width: 40px;
    height: 40px;
    animation-delay: 0s;
    animation-duration: 20s;
  }

  .circles li:nth-child(14) {
    left: 80%;
    width: 30px;
    height: 30px;
    animation-delay: 5s;
  }

  .circles li:nth-child(15) {
    left: 45%;
    width: 90px;
    height: 90px;
    animation-delay: 8s;
    animation-duration: 25s;
  }

  .circles li:nth-child(16) {
    left: 60%;
    width: 50px;
    height: 50px;
    animation-delay: 5s;
  }

  .circles li:nth-child(17) {
    left: 25%;
    width: 120px;
    height: 120px;
    animation-delay: 12s;
    animation-duration: 30s;
  }

  /* Styles for the new circles on the left */
  .circles li:nth-child(18) {
    left: 5%;
    width: 70px;
    height: 70px;
    animation-delay: 6s;
  }

  .circles li:nth-child(19) {
    left: 10%;
    width: 110px;
    height: 110px;
    animation-delay: 7s;
    animation-duration: 15s;
  }

  .circles li:nth-child(20) {
    left: 2%;
    width: 45px;
    height: 45px;
    animation-delay: 5s;
  }

  .circles li:nth-child(21) {
    left: 18%;
    width: 80px;
    height: 80px;
    animation-delay: 10s;
    animation-duration: 18s;
  }

  .circles li:nth-child(22) {
    left: 8%;
    width: 60px;
    height: 60px;
    animation-delay: 15s;
    animation-duration: 22s;
  }

  @keyframes animate {
    0% {
      transform: translateY(0) rotate(0deg);
      opacity: 1;
      border-radius: 0;
    }

    100% {
      transform: translateY(-1000px) rotate(500deg);
      opacity: 0;
      border-radius: 100%;
    }
  }
</style>
