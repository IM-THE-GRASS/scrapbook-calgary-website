<script>
  import Background from "./background.svelte";
  import Signup from "./signup.svelte";
  import Timeline15th from "./mar15.svelte";
  import Timeline16th from "./mar16.svelte";
  import Sponsors from "./sponsors.svelte";
  import { Label } from "$lib/components/ui/label";
  import Faq from "./FAQ.svelte";
  import * as Card from "$lib/components/ui/card";
</script>
<div class="flex flex-col w-full absolute top-0">
  <Background />
  <div class="flex flex-row w-full top-0">
    <div class="flex flex-col  top-0 h-100%">
      <Label class="text-4xl font-extrabold text-center mx-16 text-white mb-12">Scedule</Label>

      <div class="flex   top-0 h-100%">
        <Timeline15th />
        <Timeline16th />
      </div>
    </div>
    <Faq></Faq>
    
  </div>
  <Sponsors />
</div>
<div class="flex flex-col w-full h-[300vh] absolute"> >
  <div class="flex justify-center flex-col w-full h-screen items-center absolute">
    <img src="/assets/logo.svg" alt="Logo" class="scale-125 mt-[7vh] -mb-[7vh]"/>
    <div class="flex justify-center flex-col w-full h-screen items-center relative gap-7">
      <div class="title">
        The <span class="text-red-400 bg-slate-900 rounded-md shadow-lg p-1">highschool hackathon</span>
        where your wacky ideas
      </div>
      <div class="title">
        become <span class="text-blue-400 bg-slate-900 rounded-md shadow-lg p-1">wonderful inventions.</span>
      </div>
      <Signup />
      <div class="text-2xl font-phantom t text-center mx-16 text-white">
        March 15-16, location TDB
      </div>
    </div>
  </div>
</div>
