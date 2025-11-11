<script lang=ts>
   import {Logo} from '$lib/index.ts'
	import { MenuIcon } from 'svelte-feather-icons';
   const menus = ['Top', 'Info', 'Register','Schedule','Booklet', 'Contact']
   const ids = ['top', 'info', 'register', 'schedule','ib', 'contact']

   const scrollSection = (id: string) => {
		const element = document.getElementById(id);
		if (element) {
			element.scrollIntoView({ behavior: 'smooth' });
		}
	};
</script>

<div class="navbar w-screen hidden lg:flex bg-accent h-10">
   <div class="navbar-start">
      <a href="/">
         <img class="h-12 aspect-square" src={Logo} alt="logo">
      </a>
   </div>
   <div class="navbar-center gap-8">
      {#each menus as _, idx}
         <a href="#{ids[idx]}" on:click|preventDefault={() => scrollSection(ids[idx])}>
            <p class="text-accent-content hover:animate-bounce transition-transform">{menus[idx]}</p>
         </a>
      {/each}
   </div>
   <div class="navbar-end">
   </div>
</div>

<!-- hamburger nav bar for mobile-->
<div class="navbar w-screen lg:hidden bg-success-content h-16">
   <div class="navbar-start">
      <a href="/">
         <img class="h-12 aspect-square" src={Logo} alt="logo">
      </a>
   </div>
   <div class="navbar-end">
      <div class="dropdown dropdown-top dropdown-end">
         <label tabindex="0" class="btn btn-circle btn-ghost m-1">
            <MenuIcon size=32 />
         </label>
         <ul tabindex="0" class="menu menu-compact dropdown-content mt-3 p-2 shadow bg-base-100 rounded-box w-20">
            {#each menus as _, idx}
               <li><a href="#{ids[idx]}" on:click|preventDefault={() => scrollSection(ids[idx])}>{menus[idx]}</a></li>
            {/each}
         </ul>
      </div>
   </div>
</div>