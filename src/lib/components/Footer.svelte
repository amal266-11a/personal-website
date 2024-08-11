<script>

    import SocialMedia from "./SocialMedia.svelte";

</script>
<footer class=" bg-secondary text-secondary-foreground py-2 px-6">
    <div class=" max-w-screen-lg flex flex-col md:flex-row justify-between items-center mx-auto">   
        <span class=" self-end md:self-center">© {(new Date()).getFullYear()} by AMAL AL-SHREIF</span> 
        <div class=" flex  flex-col md:flex-row gab-4 md:gap-16">
            <span class=" flex gap-4 md:gap-0 md:flex-col items-center">
                <span class=" font-semibold">
                    Call
                </span>
                  <a href="tel:0573003184">
                    0573003184
                  </a>
                </span>
                <span class=" flex gap-4 md:gap-0 md:flex-col items-center">
                
                    <span class=" font-semibold">
                        Email
                    </span>
                      <a href="mailto:amal_266@icloud.com">
                        amal_266@icloud.com
                      </a>
                    </span>
                    <span class=" flex items-center"> <SocialMedia /> </span>
        </div>
    </div>
</footer>