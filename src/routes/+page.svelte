<script>
  import Background from "./background.svelte";
  import { Button } from "$lib/components/ui/button";
</script>

<Background />

<div class="flex justify-center flex-col w-full h-screen items-center absolute">
  <img src="/assets/logo.svg" alt="Logo" class="scale-125 mt-[7vh] -mb-[7vh]"/>
  <div class="flex justify-center flex-col w-full h-screen items-center relative gap-7">
    <div class="text-4xl font-phantom mt-[14vh] font-extrabold text-center mx-16 text-white">
      The <span class="text-red-400 bg-slate-900 rounded-md shadow-lg p-1">highschool hackathon</span>
      where your wacky ideas
    </div>
    <div class="text-4xl font-phantom font-extrabold text-center mx-16 text-white">
      become <span class="text-blue-400 bg-slate-900 rounded-md shadow-lg p-1">wonderful inventions.</span>
    </div>
    <Button variant="secondary" class=" mt-[5vh] dark text-xl scale-[1.5] text-white font-phantom font-bold hover:scale-[1.45] transition-all duration-200">Sign up now</Button>
    <div class="text-2xl font-phantom t text-center mx-16 text-white">
      March 15-16, location TDB
    </div>
  </div>
</div>
