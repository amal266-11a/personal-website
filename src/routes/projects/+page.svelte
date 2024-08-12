<script lang="ts">
    import Container from "$lib/components/Container.svelte";
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import Title from "$lib/components/Title.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    
</script>
<Container class=" flex flex-col gap-8" >
   <Title title="Project" />
<p class=" font-bold text-sm dark:text-indigo-200">
    I participated with AlCato in the Modern Frontend course,
    and I benefited a lot from it and learned new things.
    Here are the projects that I did in the course:   
</p>
<ProjectCard title="Calculator" imgsrc="/project1.png"> 
<ul class=" list-disc font-bold text-sm dark:text-violet-950 pb-5">
    <li>
    Pink design
</li>
<li>
    Easy to use interface for basic calculations
</li>
<li>
    Clear button
</li>
<li>
    Deals with invalid calculations
</li>
</ul>
<Button href="https://669343872cfa68a86ed8e665--statuesque-dolphin-bf1e49.netlify.app/">try it!</Button>
</ProjectCard>
<ProjectCard title="To Do List" imgsrc="/project2.png">
 <ul class=" list-disc font-bold text-sm dark:text-violet-950 pb-5">
    <li>Simple and easy to use design</li>
    <li>the task is entered with the addition of the time and day you want to complete the task</li>
    <li>and it can be deleted</li>
 </ul>  
 <Button  href="https://todolistamal.netlify.app/">try it!</Button> 
</ProjectCard>

</Container>