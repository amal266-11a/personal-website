<script lang="ts">
    import Container from "$lib/components/Container.svelte";
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import Title from "$lib/components/Title.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import { reveal } from 'svelte-reveal';

</script>
<Container  class=" flex flex-col gap-8" >
   <Title title="Project" />
<p use:reveal={{preset:'fly'}} class=" font-bold text-sm dark:text-indigo-200 sr__hide">
    I participated with AlCato in the Modern Frontend course,
    and I benefited a lot from it and learned new things.
    Here are the projects that I did in the course:   
</p>
<ProjectCard title="Calculator" imgsrc="/project1.png"> 
<ul use:reveal={{preset:'slide'}} class=" list-disc font-bold text-sm dark:text-violet-950 pb-5 sr__hide">
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
<Button class=" bg-indigo-300" href="https://github.com/amal266-11a/calculator.git">Source</Button>
</ProjectCard>
<ProjectCard title="To Do List" imgsrc="/project2.png">
 <ul use:reveal={{preset:'slide'}} class=" list-disc font-bold text-sm dark:text-violet-950 pb-5 sr__hide">
    <li>Simple and easy to use design</li>
    <li>the task is entered with the addition of the time and day you want to complete the task</li>
    <li>and it can be deleted</li>
 </ul>  
 <Button  href="https://todolistamal.netlify.app/">try it!</Button>
 <Button class=" bg-indigo-300" href="https://github.com/amal266-11a/todolist.git">Source</Button> 
</ProjectCard>

</Container>