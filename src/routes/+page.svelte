<script>
    import NavBar from "./_components/NavBar.svelte";
    import TopBar from "./_components/TopBar.svelte";
    import DraggableWindow from "./_components/windows/DraggableWindow.svelte";



</script>
<div class="abslute top-0 w-full">
<TopBar></TopBar>
</div>
<div class="w-full h-full">
    <DraggableWindow background="bg-neutral-800">
            <div class="cursor-default flex items-center justify-center h-full text-center" slot="header">
                <div class="flex overflow-hidden rounded bg-neutral-600 h-8 w-24">
                    <p class="text-gray-50 pt-0.5 pl-2">Cosmoshield.org</p>
                </div>
        </div>
        <div slot="content" class="w-96 h-96">
            <iframe style="width: 1500px; height: 700px" class="min-w-full min-h-full" src="https://cosmoshield.org"></iframe>
        </div>
    </DraggableWindow>
</div>
<div class="absolute bottom-0 w-full">
    <NavBar class="relative"></NavBar>
</div>
