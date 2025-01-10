<script>
  import { Button } from "$lib/components/ui/button"; 
  import * as Dialog from "$lib/components/ui/dialog";
  import { Input } from "$lib/components/ui/input";
  import { Label } from "$lib/components/ui/label";

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
    <Dialog.Content class=" bg-[#111113] border-none">
        <Dialog.Title class="font-phantom text-white text-2xl border-none">Sign Up</Dialog.Title>
            <div class="mb-4">
                <Label for="name" class="block text-[#B0B4BA] dark text-sm font-medium ">Name</Label>
                <Input id="name" type="text" class="text-white mt-1 block dark w-full border-none bg-[#18191B]" />
            </div>
            <div class="mb-4">
                <Label for="age" class="block text-[#B0B4BA] dark text-sm font-medium ">Age</Label>
                <Input id="age" type="number" class=" text-white mt-1 block dark w-full border-none bg-[#18191B]" />
            </div>
            <div class="mb-4">  
                <Label for="email" class="block text-[#B0B4BA] dark text-sm font-medium ">Email</Label>
                <Input id="email" type="email" class="text-white mt-1  dark block bg-[#18191B] w-full border-none " />
            </div>
            <div class="flex justify-end">
                <Button variant="secondary" class=" text-[#B0B4BA]  bg-[#202221] relative font-phantom dark">Submit</Button>
                <Dialog.Close>
                    <Button variant="secondary" class="text-[#B0B4BA]  bg-[#202221] relative font-phantom dark">Cancel</Button>
                </Dialog.Close>
            </div>
    </Dialog.Content>
</Dialog.Root>