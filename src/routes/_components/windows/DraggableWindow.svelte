<script>
let mouseDown = false;
let window;

export let background = "bg-gray-300";
let position = {
    x: 0,
    y: 0,
}

function startMouseHold(event){
    mouseDown = true;
    position.x = event.clientX;
    position.y = event.clientY;

}
function movingMouse(event){
    event.preventDefault();
    if (mouseDown){
        let oX = position.x;
        let oY = position.y;
        position.x = event.clientX;
        position.y = event.clientY;

        // Previous Cursor position minus current position
        let movX = oX - position.x;
        let movY = oY - position.y;
        window.style.top = (window.offsetTop - movY) + "px"
        window.style.left = (window.offsetLeft - movX) + "px"
    }
}




</script>
<style>
    .draggable {
        position: absolute;
    }
</style>
<div on:mousemove={movingMouse}
     on:mouseup={(event) => {event.preventDefault(); mouseDown = false;}}
     class="absolute">
    <div
         on:mousedown={startMouseHold}
         class="rounded-lg {background} overflow-hidden draggable" bind:this={window}>
        <div class="flex flex-col">
            <div class="flex items-center py-1">
                <div class="flex  gap-1 px-2">
                    <div class="h-4 w-4 rounded-full bg-red-700">
                    </div>
                    <div class="h-4 w-4 rounded-full bg-yellow-700">
                    </div>
                    <div class="h-4 w-4 rounded-full bg-green-700">
                    </div>
                </div>
                <div>
                    <slot name="header"></slot>
                </div>
            </div>
            <div style="width: 1500px;height: 700px" class="">
                <slot name="content">

                </slot>
            </div>
        </div>
    </div>
</div>
