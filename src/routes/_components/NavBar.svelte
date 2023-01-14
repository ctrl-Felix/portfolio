<script>
    import finder from "$lib/images/icons/finder.png"
    import mail from "$lib/images/icons/mail.png"
    import bin from "$lib/images/icons/bin.png"
    import firefox from "$lib/images/icons/firefox.png"
    import github from "$lib/images/icons/github.png"
</script>
<style>
    .blurry {
        background-color: rgba(255, 255, 255, 0.25);
    }
</style>
<div class="flex justify-center mx-auto w-full h-20 mb-2" style="backdrop-filter: blur(10px);">
    <div class="flex justify-center h-20 bg-gray-200 blurry rounded-xl mx-auto">
        <div class="h-20 w-20 opacity-100 mx-1">
            <img class="transition duration-150 ease-in-out hover:scale-125 p-0.5 h-full w-full" alt="Finder icon" src={finder}/>
        </div>
        <div class="h-20 w-20 opacity-100 mx-1">
            <img class="transition duration-150 ease-in-out hover:scale-125 p-0.5 h-full w-full" alt="Finder icon" src={mail}/>
        </div>
        <div class="h-20 w-20 opacity-100 mx-1">
            <img class="transition duration-150 ease-in-out hover:scale-125 p-0.5 h-full w-full" alt="Finder icon" src={firefox}/>
        </div>
        <div class="h-20 w-20 opacity-100 mx-1">
            <img class="transition duration-150 ease-in-out hover:scale-125 p-0.5 h-full w-full" alt="Finder icon" src={github}/>
        </div>
        <div class="w-0.5 h-16 mt-2 bg-gray-200 opacity-30"></div>
        <div class="h-20 w-20 opacity-100 mx-2 my-auto">
            <img class="transition duration-150 ease-in-out hover:scale-125 p-0.5 h-full w-full" alt="Finder icon" src={bin}/>
        </div>


    </div>
</div>