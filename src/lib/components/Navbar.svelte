<script lang="ts">
import Button from "./ui/button/button.svelte";
import { page} from "$app/stores";
import * as Sheet from "$lib/components/ui/sheet";
    import ThemeSwitch from "./ThemeSwitch.svelte";
const links = [
    {
        text: "ABOUT ME",
        href: "/",
    },
    {
        text: "RESUME",
        href: "/resume",
    },
    {
        text: "PROJECTE",
        href: "/projects",
    },
    {
        text: "CONTACT",
        href: "/contact",
    }
    ];
    let isSheetOpen=false;
</script>

<div class=" bg-secondary text-secondary-foreground py-8 px-6">
    <nav class=" max-w-screen-lg flex justify-between items-center mx-auto">

        <div class=" flex items-center gap-2 ">
     <div class=" bg-primary w-5 h-5 me-4"/>
    
    <div class=" flex items-center gap-2">
    
        <span class=" font-bold text-3xl">
            Amal 
         </span>
         <span class=" text-xl uppercase">
           / Web Developer  
         </span>
    
        </div>   
 </div>
   <div class=" flex">
    <ThemeSwitch />
    <!-- large scrren -->
    <div class=" hidden lg:flex">
        {#each links as link }
                <Button class=" {$page.url.pathname == link.href && "text-primary"}" href={link.href} variant="link" on:click={() => isSheetOpen = false}>
                 {link.text}
                   </Button>
                {/each}  
        </div>
        <!-- small screen -->
        <Sheet.Root bind:open={isSheetOpen}>
            <Sheet.Trigger class="flex lg:hidden">
                <Button  variant="ghost" size="icon">
                <svg class="w-6 h-auto" xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 2048 2048"><path fill="currentColor" d="M2048 768v128h-878q-36-118-72-233t-74-234q-37 118-73 233t-73 234H376q102 78 202 156t203 155q-40 124-78 246t-76 247l397-306v162l-640 492l248-794L0 768h784L1024 0l240 768zm-896 384h896v128h-896zm0 384h896v128h-896z"/></svg>   
            </Button>
        </Sheet.Trigger>
            <Sheet.Content class=" flex flex-col justify-center">
                {#each links as link }
                <Button class=" text-xl {$page.url.pathname == link.href && "text-primary"}" href={link.href} variant="link" on:click={() => isSheetOpen = false}>
                 {link.text}
                   </Button>
                   
                    
                {/each} 
            </Sheet.Content>
          </Sheet.Root>
       
          
   </div>
          </nav>
                </div>