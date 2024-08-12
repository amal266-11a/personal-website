<script lang="ts">
 
 export let title: string;
export let imgsrc:string;
 
</script>





<div class=" bg-secondary  shadow-xl  flex flex-col sm:flex-row gap-4 justify-between">
   
    <div class="flex flex-col  gap-16 pt-9">
        <div class=" flex flex-col min-w-32 border-s-8 border-primary ps-8">
            <span class=" text-primary text-xl font-bold ">{title}</span>
         </div>
            <div class="ps-8">
                 <slot />
                 
             </div>
    </div>
         <img src="{imgsrc}" alt="صوره للمشروع" class="w-auto sm:w-64 object-center"/>

   </div>
   