<script>
  import Title from "$lib/componenten/Title.svelte";

  import { onMount } from "svelte";

  let cursor;

  onMount(() => {
    document.addEventListener("mousemove", handleMouseMove);
    document.addEventListener("click", handleMouseClick);

    return () => {
      document.removeEventListener("mousemove", handleMouseMove);
      document.removeEventListener("click", handleMouseClick);
    };
  });

  function handleMouseMove(e) {
    cursor.style.transform = `translate(${e.clientX - 10}px, ${
      e.clientY - 10
    }px)`;
  }

  function handleMouseClick(e) {
    const clickOverlay = document.getElementById("click");
    const leave = document.getElementById("leave");

    // the position of the leave based on the click coordinates
    leave.style.left = `${e.clientX - leave.offsetWidth / 1}px`;
    leave.style.top = `${e.clientY - leave.offsetHeight / 1}px`;
    clickOverlay.style.display = "flex";

    setTimeout(() => {
      clickOverlay.style.display = "none";
    }, 1000);
  }
</script>

<main>
  <Title />

  <div bind:this={cursor} class="burlesque-cursor"></div>
  <div id="click">
    <img src="src/lib/assets/leave.png" alt="leave" id="leave" />
  </div>

</main>
<style>
  .burlesque-cursor {
    position: absolute;
    width: 30px;
    height: 30px;
    background-color: var(--background-color);
    border-radius: 50%;
    transition: transform 2s ease-out;
  }

  .burlesque-cursor::before {
    content: "";
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: var(--background-color-light);
    border-radius: 50%;
    top: 40%;
    left: 20%;
    transform: translate(-50%, -50%);
    z-index: -1;
  }

  #click {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: none;
    justify-content: center;
    align-items: center;
    background: none;
  }

  #leave {
    position: absolute;
    width: 48px;
    height: 48px;
    fill: var(--background-color);
  }
</style>
