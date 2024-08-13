<script>
import { reveal } from 'svelte-reveal';

    import Container from "$lib/components/Container.svelte";
import Title from "$lib/components/Title.svelte";
import Button from "$lib/components/ui/button/button.svelte";
import ResumeCard from "$lib/components/ResumeCard.svelte";
</script>
<Container class="" >
    <Title title="Resume" />
    <div use:reveal={{preset:'slide'}} class="pt-16 flex flex-col gap-8 sr__hide">
<div class=" flex justify-between items-center">
    <span class=" text-2xl font-bold">Education</span>

</div  >
 
<ResumeCard  date="2023-presnt" title="computer scince Bachelor" company="Umm Al-Qura University"  />
 </div>
    
</Container>