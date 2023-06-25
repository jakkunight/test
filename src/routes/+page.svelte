<script>
    let count = 0;
    let msg = "Púlsame!"
    const handleClick = (event) => {
        count = count + 1;
        msg = "Me han pulsado " + count + " veces!";
    };
    console.log("[INFO] Base path: " + process.env.BASE_URL);
</script>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<button on:click={handleClick}>
    {msg}
</button>