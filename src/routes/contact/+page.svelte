<script>
    import Container from "$lib/components/Container.svelte";
    import Title from "$lib/components/Title.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
import  {Input}  from "$lib/components/ui/input";
import  {Label}  from "$lib/components/ui/label";
    import Textarea from "$lib/components/ui/textarea/textarea.svelte";
</script>
<Container class=" flex flex-col gap-16">
    <Title title="Let's Talk" />
    <form action="https://formsubmit.co/amal_266@icloud.com" method="POST"
      class=" bg-secondary  p-8 flex flex-col gap-8">
        <div>
        <Label for="name" class=" text-secondary-foreground">Full Name</Label>
        <Input required name="name" id="name" placeholder="write your name!"/>
        </div>
        <div>
            <Label for="email" class=" text-secondary-foreground">Email</Label>
            <Input required type="email" name="email" id="email" placeholder="example@xyz.abc"/>
            </div>
            <div>
                <Label for="subject" class=" text-secondary-foreground">Subject</Label>
                <Input required name="subject" id="subject" placeholder="....."/>
                </div>
                <div>
                    <Label for="message" class=" text-secondary-foreground">Message</Label>
                    <Textarea required  name="message" id="message" placeholder="....."/>
                    </div>
                    <Button class="max-w-32" type="submit">
                     submit
                    </Button>
    </form>
</Container>