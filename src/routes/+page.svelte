<script>
  import Background from "./background.svelte";
  import { Button } from "$lib/components/ui/button";
</script>

<Background />

<div class="flex justify-center flex-col w-full h-screen items-center absolute">
  <img src="/assets/logo.svg" alt="Logo" class="scale-150  translate-y-500 mt-[15vh]"/>
  <div class="flex justify-center flex-col w-full h-screen items-center relative gap-7">
    <div class="text-4xl font-phantom font-extrabold text-center mx-16 text-white">
      The <span class="text-red-400 bg-slate-900 rounded-md shadow-lg p-1">highschool hackathon</span>
      where your wacky ideas
    </div>
    <div class="text-4xl font-phantom font-extrabold text-center mx-16 text-white">
      become <span class="text-blue-400 bg-slate-900 rounded-md shadow-lg p-1">wonderful inventions.</span>
    </div>
    <Button variant="secondary" class="dark text-xl scale-150 text-white font-phantom font-bold hover:scale-105 transition-all duration-300 ">Sign up now</Button>
  </div>
</div>
