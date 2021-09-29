<script>
  import darkMode from "./DarkMode.svelte";
</script>

{#if darkMode === true}
  <img
    src="FullblackLogo_with_text.svg"
    alt="lightning mail logo"
    width="12%"
    height="12%"
  />
{:else}
  <img
    src="DefaultLogo_with_text.svg"
    alt="lightning mail logo"
    width="12%"
    height="12%"
  />
{/if}

<style type="text/scss">
</style>
