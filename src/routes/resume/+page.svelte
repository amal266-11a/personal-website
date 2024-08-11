<script>

    import Container from "$lib/components/Container.svelte";
import Title from "$lib/components/Title.svelte";
import Button from "$lib/components/ui/button/button.svelte";
import ResumeCard from "$lib/components/ResumeCard.svelte";
</script>
<Container className="" >
    <Title title="Resume" />
    <div class="pt-16 flex flex-col gap-8">
<div class=" flex justify-between items-center">
    <span class=" text-2xl font-bold">Education</span>

</div>
 
<ResumeCard date="2023-presnt" title="computer scince Bachelor" company="Umm Al-Qura University"  />
 </div>
    
</Container>