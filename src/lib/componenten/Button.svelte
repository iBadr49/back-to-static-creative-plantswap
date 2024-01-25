<!-- Button.svelte -->
<script>
  export let href = "/";
  export let label = "Button";
</script>

<a {href}>{label}</a>

<style>
  a {
    display: inline-block;
    padding: 10px 20px;
    margin: 10px;
    text-decoration: none;
    color: black;
    background-color: var(--button-color);
    border: 2px solid var(--background-color);
    border-radius: 8px;
    transition:
      background-color 0.3s ease,
      color 0.3s ease;
  }

  a:hover {
    background-color: var(--background-color);
    border: 2px solid var(--button-color);
    color: #fff;
  }
</style>
