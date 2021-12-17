<script lang="ts">
  import { link } from 'svelte-spa-router'
</script>

<main class="h-screen relative">

  <div class="h-screen absolute top-0 overflow-x-hidden">
    <div class="bg-blue-200 relative h-1/2">
      <img src="flower_ume.png" alt="ume." class="absolute h-1/2 bottom-0 left-0 animate-spin"/>
      <img src="flower_ume.png" alt="ume." class="absolute h-1/2 bottom-0 right-0 animate-spin"/>
    </div>
    <div class="h-1/2">
      <img src="ishidatami.jpg" alt="ishidatami." class="object-cover w-full h-full"/>
    </div>
  </div>

  <div class="h-screen relative">
    <div class="pt-12 flex justify-center">
      <img src="happy_new_year.png" alt="happy_new_year." class="animate-pulse" />
    </div>
    <div class="flex justify-center">
        <img src="jinja.png" alt="jinja." />
    </div>
    <div class="flex justify-center absolute bottom-0 pb-4" >
      <img src="man.png" alt="man." class="object-fit w-1/4 p-1" />
      <a href={"/result"} use:link class="w-1/2 p-1">
        <img src="omikuji.png" alt="omikuji." class="object-fit animate-bounce" />
      </a>
      <img src="woman.png" alt="woman." class="object-cover w-1/4 p-1" />
    </div>
  </div>


</main>