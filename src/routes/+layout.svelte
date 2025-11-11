<script lang="ts">
	import '../app.css'
   import { onMount } from 'svelte';
	import favicon from '$lib/assets/favicon.svg'
	import Navbar from "$lib/Navbar.svelte";
	import { fade } from 'svelte/transition';
	import { ChevronUpIcon } from "svelte-feather-icons";

	let showScroll: boolean = $state(false);
   const onScroll = () => {
   	showScroll = (window.scrollY || document.documentElement.scrollTop) > 200;
   };
   const scrollToTop = () => window.scrollTo({ top: 0, behavior: 'smooth' });
	onMount(() => {
     onScroll();
     window.addEventListener('scroll', onScroll);
     return () => window.removeEventListener('scroll', onScroll);
   });

	let { children } = $props()
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<header class="w-screen fixed overflow-x-clip bottom-0 lg:top-0 h-fit z-20">
	<Navbar/>
</header>


<main class="overflow-x-clip" id="main">
	<div>
	{@render children()}
	</div>
</main>

{#if showScroll}
<button
  class="hidden lg:block fixed bottom-4 right-4 z-50 p-3 rounded-full bg-blue-600 hover:bg-blue-700 hover:-translate-y-2 duration-200 text-white shadow-lg" in:fade out:fade
  onclick={scrollToTop}
  aria-label="Scroll to top"
  title="Scroll to top"
>
  <ChevronUpIcon size=24 />
</button>
{/if}