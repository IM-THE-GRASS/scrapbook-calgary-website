<script>
  import Background from "./background.svelte";
  import Signup from "./signup.svelte";
  import Timeline15th from "./mar15.svelte";
  import Timeline16th from "./mar16.svelte";
  import * as Card from "$lib/components/ui/card";
  const FAQs = [
      { title: 'Doors open', description: '8:30 am' },
      { title: 'Opening ceremony', description: '9:00 am' },
      { title: 'Code', description: '09:30 pm' },
      { title: 'Lunch', description: '12:00 pm' },
      { title: 'Code', description: '01:00 pm' },
      { title: 'Dinner', description: '06:00 pm' },
      { title: 'Code', description: '07:00 pm' },
      { title: 'Sleep', description: 'NEVER' },
  ];
</script>
<div class="flex flex-col w-full absolute top-0">
  <Background />
  <div class="flex flex-row w-full top-0">
    <Timeline15th />
    <Timeline16th />
    <div class="flex flex-wrap flex-row w-full top-0 h-100%">
      {#each FAQs as FAQ}
        <Card.Root class="w-[10vw] h-[20vh] bg-[#111113] border-none m-20">
          <Card.Title class="title">{FAQ.title}</Card.Title>
          <Card.Content class="label">{FAQ.description}
          </Card.Content>
        </Card.Root>
      {/each}
    </div>
  </div>
  

</div>
<div class="flex flex-col w-full h-[300vh] absolute">
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
