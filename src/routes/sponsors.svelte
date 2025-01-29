<script>
    import * as Card from '$lib/components/ui/card';
    const Sponsors = [
        { title: 'ARC', description: 'Alpine Reasoning Challenge is a non-profit, youth-led organization based in Calgary, committed to nurturing young minds and encouraging a deep passion for education. Our contests serve as a platform for students to showcase their problem-solving abilities, critical thinking skills, and creativity. At ARC, We firmly believe that nurturing talent in STEM and the arts can shape a brighter future for mathematics, coding, science, and humanities.', rank: '', image:'https://static.wixstatic.com/media/7f1f50_a9b71b1c3dd44979a6f4747b0099e722~mv2.png/v1/fill/w_460,h_463,al_c,q_85,usm_0.66_1.00_0.01,enc_avif,quality_auto/ARC_logo.png'},
        { title: 'Hack Club', description: "Hack Club is a global community of thousands of high school makers. We're organizers, coders, hackers, painters, engineers, musicians, writers, volunteers. We make things. We want others to make things too.", rank: '', image:'https://assets.hackclub.com/icon-rounded.png'},
        { title: 'CoFlex', description: 'CoFlex hosts a diverse range of professionals, from freelancers to startups, fostering uniqe connections and cross-industry networking opportunities.', rank: '', image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRAzhpZLl36tXw_nPUv-bCRnkmbyoSyGdc4nQ&s'},

    ];
</script>



    
<div class="relative">
    <Card.Root class="card">
        <Card.Title class="title my-">Sponsors</Card.Title> 
        <div class="flex flex-row flex-wrap justify-center">
            {#each Sponsors as Sponsor}
            <Card.Root class="w-[31vw] card">
                <Card.Title class="subtitle text-4xl font-extrabold font-phantom mx-5">{Sponsor.title}</Card.Title>  
                <Card.Title class="subtitle mt=5">{Sponsor.rank}</Card.Title>
                <img src={Sponsor.image} alt="Sponsor logo" class="mx-[10%] my-5 rounded-md place-self-center w-[460px] h-[460px]"/>
                <Card.Content class="label">
                    {Sponsor.description}
                </Card.Content>
            </Card.Root>
            {/each} 
        </div>

        
    </Card.Root>
</div>
