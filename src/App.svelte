<script lang="ts">
  import { Router, Route, Link } from "svelte-routing";
  import Experience from "./pages/Experience.svelte";
  import Header from "./pages/Header.svelte";
  import Landing from "./pages/Landing.svelte";
  import Footer from "./pages/Footer.svelte";
  export let url = ""; //This property is necessary declare to avoid ignore the Router
</script>

<main>
  <Router {url}>
    <Header />
    <div class="content">
      <Route path="/" component={Landing} />
      <Route path="/work" component={Experience} />
    </div>
    <Footer />
  </Router>
</main>

<style>
  main {
    text-align: center;
    max-width: 240px;
    height: 100%;
    margin: 0 auto;
    min-height: 0;
    display: flex;
    flex-direction: column;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  .content {
    height: 100%;
    min-height: 0;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
