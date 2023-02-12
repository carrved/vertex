<script>
  import { slide, scale } from 'svelte/transition';
  import { onMount } from 'svelte';

  function discord() {
    window.open("https://discord.gg/VjA6cu6v3c", '_blank').focus();
  }

  let ready = false;
  onMount(() => ready = true);
</script>
{#if ready}
<main in:scale="{{ duration: 1500 }}">
  <img class="title floating" src="https://www.simpleimageresizer.com/_uploads/photos/9b0097ae/vertex2_2_75.png"/>
  <h3 style="font-family: 'Krona One', sans-serif;">The best free executor on the market.</h3>
  
  <button on:click={discord}>discord</button>
  <button>purchase</button>
</main>
{/if}

<style>
</style>
