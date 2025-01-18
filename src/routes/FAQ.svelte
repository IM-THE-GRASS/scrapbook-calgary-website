<script>
    import { Label } from "$lib/components/ui/label";
    import * as Card from "$lib/components/ui/card";
    const FAQs = [
        { title: 'What is Scrapyard?', description: "Scrapyard is a global hackathon running in Los Angeles and 100+ other cities by high schoolers (like Counterspell) with a “scrappy” theme of stupid inventions! It's organized by Hack Club, a 501(c)(3) nonprofit that supports a global community of 48k high school makers." },
        { title: 'Who can participate in Scrapyard?', description: "All high-school & upper-middle-school aged students are welcome to come! You don't have to be a member of the Hack Club community or be a Hack Club leader." },
        { title: 'I’m not good at coding. Can I still participate?', description: "This hackathon is for creatives of all skill levels! We'll have workshops and other events so join us and let's learn together. If you'd like to start exploring some introductory projects, check out Hack Club Workshops." },
        { title: 'What can I make at Scrapyard?', description: 'The scrappiest thing you can imagine –- jank is encouraged. Games? Apps? Websites? Programming languages? Hardware? You name it! We’ll have a bunch of resources and mentors to help you out.' },
    ];
</script>
<div class="flex flex-wrap flex-row w-full top-0 h-100%">
    <Label class="text-4xl font-extrabold text-center mx-16 text-white w-full">FAQ</Label>
    {#each FAQs as FAQ}
      <Card.Root class="w-[48%]  card">
        <Card.Title class="subtitle font-phantom">{FAQ.title}</Card.Title>
        <Card.Content class="label">{FAQ.description}
        </Card.Content>
      </Card.Root>
    {/each}
</div>