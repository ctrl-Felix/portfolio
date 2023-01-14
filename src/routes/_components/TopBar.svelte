<script>
import apple_apple from "$lib/images/icons/apple_apple.svg"
import Hoverable from "./util/Hoverable.svelte";
</script>

<div class="p-1 bg-gray-300">
    <div class="flex justify-between w-full">
        <div class="flex space-x-3">
            <img class="h-5" src={apple_apple} alt="Apple logo"/>
            <div class="group cursor-pointer group relative">
                <p>File</p>
                    <div class="invisible group-hover:visible absolute">
                        <div class="rounded bg-gray-300 overflow-hidden mt-2 w-36">
                            <p class="pt-1 px-1 hover:bg-gray-400">Open new File</p>
                            <p class="px-1 hover:bg-gray-400">Open new File</p>
                            <p class="px-1 hover:bg-gray-400">Open new File</p>
                            <p class="px-1 pb-1 hover:bg-gray-400">Open new File</p>
                        </div>
                    </div>
            </div>
            <p>Edit</p>
            <p>View</p>
            <p>History</p>
            <p>Bookmarks</p>
            <p>Window</p>
            <p>Help</p>
        </div>
        <div class="flex space-x-3">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M8.288 15.038a5.25 5.25 0 017.424 0M5.106 11.856c3.807-3.808 9.98-3.808 13.788 0M1.924 8.674c5.565-5.565 14.587-5.565 20.152 0M12.53 18.22l-.53.53-.53-.53a.75.75 0 011.06 0z" />
            </svg>
            <p>Tue Oct 18 9:51 AM</p>
        </div>

    </div>
</div>