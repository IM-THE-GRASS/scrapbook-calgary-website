<script>
  import { Button } from "$lib/components/ui/button"; 
  import * as Dialog from "$lib/components/ui/dialog";
  import { Input } from "$lib/components/ui/input";

</script>


<Dialog.Root>
    <Dialog.Trigger>
        <Button 
            variant="secondary" 
            class="mt-[5vh] dark text-xl scale-[1.5] text-white relative font-phantom font-bold hover:scale-[1.45] transition-all duration-200"
        >
            Sign up now
        </Button>
    </Dialog.Trigger>
    <Dialog.Content class=" bg-[#111113] border-none min-w-[70vw] max-h-[90vh]">
        <iframe src="https://forms.hackclub.com/scrapyard-signup?event=calgary" class="w-full max-h-[90vh]" title="Signup Form"></iframe>
    </Dialog.Content>
</Dialog.Root>
