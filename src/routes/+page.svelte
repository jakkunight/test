<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<script>
    let count = 0;
    let msg = "Púlsame!"
    const handleClick = (event) => {
        count = count + 1;
        msg = "Me han pulsado " + count + " veces!";
    };
</script>
<button on:click={handleClick}>
    {msg}
</button>