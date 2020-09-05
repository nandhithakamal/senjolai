<script>
  import Tailwindcss from "./Tailwindcss.svelte";
  import Navbar from "./navbar.svelte";

  export let name;
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  body {
    background-image: url("https://www.balcanicaucaso.org/var/obc/storage/images/zone/bosna-i-hercegovina/poljoprivreda-i-ruralna-podrucja-zapadnog-balkana-zemlje-poljoprivrede-i-ruralnog-razvoja-95798/585748-2-ita-IT/Agriculture-and-rural-areas-in-the-Western-Balkans-status-update.jpg");
    height: 500px;
    background-color: #cccccc;
    /* background-position: center; */
    background-repeat: no-repeat;
    background-size: cover;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<Tailwindcss />

<body>
  <div class="bg"></div>
  <Navbar />
  <main>
    <h1>Hello {name}!</h1>
    <p>
      Visit the
      <a href="https://svelte.dev/tutorial">Svelte tutorial</a>
      to learn how to build Svelte apps.
    </p>
  </main>
</body>