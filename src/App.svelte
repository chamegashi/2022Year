<script lang="ts">
  import Tailwindcss from './Tailwindcss.svelte';
  import Router from 'svelte-spa-router'
  import { routes } from './router'
</script>

<Tailwindcss />
<main>
  <Router {routes} />
</main>