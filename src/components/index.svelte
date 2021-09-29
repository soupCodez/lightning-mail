<script>
  import Toggle from "../components/DarkMode.svelte";
  import Logo from "../components/Logo.svelte";
</script>

<svelte:head>
  <link
    href="https://fonts.googleapis.com/icon?family=Material+Icons"
    rel="stylesheet"
  />
  <title>Sapper project template</title>
</svelte:head>

<body>
  <Logo />
  <Toggle />
  <img
    src="undraw_email.svg"
    alt="undraw personal email"
    width="30%"
    height="30%"
  />
  <h1>The Best <span class="highlighted-text">E-Mail</span> Marketing Tool!</h1>

  <p>YES</p>
</body>

<style type="text/scss">
  @import url("https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@800&display=swap");

  $light: #ffffff;
  $dark: #212121;
  $accent-color: #536dfe;

  ::root {
    --bgcolor: #{$light};
    --textcolor: #{$dark};
  }

  :global(body) {
    background: var(--bgcolor);
    color: var(--textcolor);
  }

  :global(body.dark) {
    --bgcolor: #{$dark};
    --textcolor: #{$light};
  }

  img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 1%;
    margin-top: 1%;
  }

  .highlighted-text {
    color: $accent-color;
  }

  body {
    background: var(--bgcolor);
    color: var(--textcolor);
  }

  * {
    background: var(--bgcolor);
    color: var(--textcolor);
    font-family: "Nunito Sans", sans-serif;
  }

  h1,
  p {
    text-align: center;
    margin: 0 auto;
  }

  h1 {
    font-family: "Nunito Sans", sans-serif;
    text-align: center;
    font-size: 2em;
  }

  p {
    margin: 1em auto;
  }

  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }
</style>
