<script>
    $:innerWidth = 1920;
    $:innerHeight = 1080;
</script>

<svelte:window bind:innerWidth bind:innerHeight/>

<!-- Hello, Taylor Tabb. -->
<title>Taylor Tab</title>

 {#if innerWidth >= innerHeight}
    <img 
        src="/Taylor_Tabb.png"
        alt="Taylor Tabb"
        style="width: 100vh;"
    >
{:else}
    <img 
        src="/Taylor_Tabb.png"
        alt="Taylor Tabb"
        style="width: 100vw;"
    >
 {/if}

<style>
    img{
        position: absolute;
		left: 50%;
        bottom: 0%;
		transform: translateX(-50%);
    }
</style>