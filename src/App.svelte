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

  h1{
    color: #ff5300;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<Tailwindcss />

<body class="antialiased">
  <div class="bg"></div>
  <Navbar />
  <main>
    <div class="px-4 text-center">
      <div class="max-w-3xl bg-indigo-100 rounded-lg mx-auto my-16 p-16">
        <h1 class = "text-2xl mb-2 tracking-wide font-medium">
          Welcome to Senjolai!
        </h1>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis laudantium sed autem quo deleniti eius, accusantium iure dignissimos quasi minima cum fugiat expedita et voluptatibus molestias. Magnam incidunt fugit reiciendis!
      </div>
    </div>
  </main>
</body>