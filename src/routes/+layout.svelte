<script>
    import Header from "$lib/components/Header.svelte";
    import { fly } from 'svelte/transition';
    import { page } from '$app/stores';

  const { children } = $props();

  const startTransition = () => {
      document.body.classList.add('page-transitioning');
  };

  const endTransition = () => {
      document.body.classList.remove('page-transitioning');
  };
</script>


<Header />

{#key $page.url}
  <main
      in:fly={{ x: -200, duration: 300, delay: 300 }}
      out:fly={{ x: 200, duration: 300 }}
      onintrostart={startTransition}
      onintroend={endTransition}
      onoutrostart={startTransition}
      onoutroend={endTransition}
  >
      {@render children()}
  </main>
{/key}

<style>
  :global(body) {
      width: 100%;
      min-height: 100vh;
      margin: 0;
      padding: 0;
      overflow: visible;
      font-family: Arial, sans-serif;
      box-sizing: border-box;
  }

  main {
      min-height: 100vh;
      width: 100%; 
      margin: auto;
      box-sizing: border-box;
  }
</style>