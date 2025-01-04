<script>
  import "@fontsource/geist-mono";
  import Header from "./lib/components/Header.svelte";
  import Hero from "./lib/components/Hero.svelte";
  import Features from "./lib/components/Features.svelte";
  import HowItWorks from "./lib/components/HowItWorks.svelte";
  import Contact from "./lib/components/Contact.svelte";
  import Footer from "./lib/components/Footer.svelte";
</script>

<main class="font-mono">
  <Header />
  <Hero />
  <Features />
  <HowItWorks />
  <Contact />
  <Footer />
</main>

<style>
  :global(html) {
    scroll-behavior: smooth;
  }
</style>