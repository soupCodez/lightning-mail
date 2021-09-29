<script>
  export let darkMode = false;
  const toggle = () => {
    if (darkMode === false) {
      darkMode = true;
    } else {
      darkMode = false;
    }
    window.document.body.classList.toggle("dark");
  };
</script>

<button on:click={toggle}>
  {#if darkMode === true}
    <span class="material-icons">light_mode</span>
  {:else}
    <span class="material-icons">dark_mode</span>
  {/if}
</button>

<style type="text/scss">
  button {
    float: right;
    background-color: #ffffff;
    color: black;
    border: none;
    border-radius: 4px;
    padding: 0.5rem;
    text-transform: uppercase;
  }
  :global(body.dark) button {
    background-color: #212121;
    color: white;
  }
</style>
