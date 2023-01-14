<script>
    import "../app.css"
    import img from "$lib/images/10-14-Mojave-6.jpg"

</script>
<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Meera+Inimai&display=swap" rel="stylesheet">
</svelte:head>
<style>

    @font-face {
        font-family: "San Francisco";
        font-weight: 400;
        src: url('fonts/sfapple.ttf');
    }

    .apple-font {
        font-family: "San Francisco", sans-serif;
    }

    .font {
        font-family: 'Meera Inimai', sans-serif;
    }

    .mac-background {
        background-repeat: no-repeat;
        background-attachment: fixed;
        background-position: center center;
        background-clip: border-box;
        background-origin: padding-box;
        -moz-background-size: cover;
        background-size: cover;
    }
</style>

<div class="apple-font h-screen w-screen overflow-hidden mac-background" style="background-image: url({img});">
<slot></slot>
</div>