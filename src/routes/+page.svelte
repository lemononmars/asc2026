<script lang=ts>
	import Head from '$lib/Head.svelte';
   // import { resolve } from '$app/paths';
   import { SudokuStationLogo, DiscordLogo, Logo } from '$lib';
   import {MailIcon, DownloadIcon} from 'svelte-feather-icons'
</script>

<Head title="Asian Sudoku Championship 2026" description="7th Asian Sudoku Championship" url="https://lemononmars.github.io/asc2026"></Head>

<div class="flex flex-col gap-2 my-4">
   <h1 id="top">Asian Sudoku Championship 2026</h1>
   <div class="divider"></div>

   <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTTeFd8Ze7Eou_nNxab2W-6-hpJs-hPeENzIT732pD45BVioT2tEUYabRSRmmmNVLaKLnhQi_m7y_lp/pubembed?start=false&loop=false&delayms=60000" frameborder="0" width="960" height="569" title="asc2026presentation"></iframe>

   <div class="divider"></div>
   <h3>Welcome to the official website of the 7th Asian Sudoku Championship (ASC).</h3>
   <div class="divider"></div>


   <h2 id="info">Info</h2>
   <div class="text-left">
      <ul>
         <li>Date: 7-9 February 2026</li>
         <li>Location: Rembrandt Hotel Bangkok, Bangkok, Thailand <a href="https://maps.app.goo.gl/THBQPtdHi9jRqQ3YA" target="blank_">(map)</a></li>
         <li>Divisions:
            <ul class="px-10 list-[circle]">
               <li>Individual</li>
                  <ul class="mx-10 list-[square]   ">
                     <li>U8</li>
                     <li>U10</li>
                     <li>U12</li>
                     <li>U15</li>
                     <li>U18</li>
                     <li>Casual</li>
                     <li>Master</li>
                  </ul>
               <li>Team</li>
                  <ul class="mx-10 list-[square]">
                     <li>Casual</li>
                     <li>Master</li>
                  </ul>
            </ul>
         </li>
         <div class="collapse collapse-arrow bg-base-100 border border-base-300">
               <input type="radio" name="my-accordion-2" />
               <div class="collapse-title font-semibold">Restriction</div>
               <div class="collapse-content text-sm">
                  <ul class="list-square px-10">
                     <li>U8: Under 8 years old (born on or after 1 January 2018)</li>
                     <li>U10: Under 10 years old (born on or after 1 January 2016)</li>
                     <li>U12: Under 12 years old (born on or after 1 January 2014)</li>
                     <li>U15: Under 15 years old (born on or after 1 January 2011)</li>
                     <li>U18: Under 18 years old (born on or after 1 January 2008)</li>
                     <li>Open: No age restriction</li>
                     <li>Participants ranked 1-100 in the WPF Sudoku Grand Prix <a href="https://gp.worldpuzzle.org/content/wpf-gp-sudoku-results-2024" target="blank_">2024</a> or <a href="https://gp.worldpuzzle.org/content/wpf-gp-sudoku-results-2025" target="blank_">2025</a>, must compete in the open division, regardless of their age.</li>
                     <li>Participants may compete in any higher division (e.g. a 14-year-old participant may choose the U18 division.)</li>
                  </ul>
               </div>
            </div>
      </ul>
   </div>

   <div class="divider"></div>
   <h2 id="register">Registration</h2>
   <div class=text-left>
      <ul>
         <li><span class="text-accent">Fee</span>: 7,500 THB (double), 10,500 THB (single)</li>
         <li><span class="text-accent">Deadline</span>: Sat, 20 Dec 2025</li>
         <li><span class="text-accent">Late registration</span>: Sat, 5 Jan 2026 (+10% fee)</li>
         <li><span class="text-accent">Register & payment</span>: via e-mail <a href="mailto:asc2026.tha@gmail.com" target="blank_">asc2026.tha@gmail.com</a></li>
         <li><span class="text-accent">Registration form</span>: <a href="https://drive.google.com/drive/folders/14tym-q_OJ_Ge0n0LO-81MT_fVDv5kgjU?usp=drive_link" target="blank_"> Download </a></li>
      </ul>
   </div>

   <!-- <div class="divider"></div>
   <h2 id="schedule">Schedule</h2>

   <div class="divider"></div>
   <h2 id="ib">Instruction Booklet</h2>
   
   <div class="text-left">
      <ul>
         <li>U8</li>
         <li>U10</li>
         <li>U12</li>
         <li>U15</li>
         <li>U18</li>
         <li>Casual</li>
         <li>Master</li>
      </ul>
   </div> -->

   <!-- <div class="divider"></div>
   <h2 id="faq">FAQ</h2>
      <div class="collapse collapse-arrow bg-base-100 border border-base-300">
         <input type="radio" name="my-accordion-2" />
         <div class="collapse-title font-semibold"></div>
         <div class="collapse-content text-sm">Sudoku Station</div>
      </div>
      <div class="collapse collapse-arrow bg-base-100 border border-base-300">
         <input type="radio" name="my-accordion-2" />
         <div class="collapse-title font-semibold">Logic puzzles?</div>
         <div class="collapse-content text-sm">Maybe</div>
      </div>
      <div class="collapse collapse-arrow bg-base-100 border border-base-300">
         <input type="radio" name="my-accordion-2" />
         <div class="collapse-title font-semibold">Easy</div>
         <div class="collapse-content text-sm">:(</div>
      </div> -->

   <div class="divider"></div>
   <h2 id="contact">Contact</h2>
   <div class=text-left>
      <div class="flex flex-row place-content-around gap-4 m-4">
         <!-- <div class="flex flex-col place-items-center gap-4">
            <a href="https://m.me/SudokuStation" target="_blank">
               <img src={SudokuStationLogo} alt="Sudoku Station" class="h-12"/>
               <span>Sudoku Station (messenger)</span>
            </a>
         </div> -->
      
         <a href="https://discord.gg/wbcNqYJQXJ" target="_blank">
            <div class="flex flex-col place-items-center gap-4">
               <img src={DiscordLogo} alt="Discord" class="h-12"/>
               <span>ASC2026 Discord</span>
            </div>
         </a>

         <a href="mailto:asc2026.tha@gmail.com" target="_blank">
            <div class="flex flex-col place-items-center gap-4">
               <MailIcon size=45/>
               <span>asc2026.tha@gmail.com</span>
            </div>
         </a>
      </div>
   </div>

   <div class="divider"></div>
</div>