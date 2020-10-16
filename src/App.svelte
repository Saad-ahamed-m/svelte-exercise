<script>
    // TODO: Add other states for the application
    let username = "";

    function handleClick() {
        // TODO: Add username and password value in the API call body
        // TODO: Handle Success & Failure response
    }
</script>

<style>
    /* TODO: Add Styles to application  */
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>

<main>
    <h4>Login Form!</h4>
    <div>
        <!-- TODO: Conditional Rendering based on the API call response -->
        <input type="text" placeholder="Username" bind:value={username} />
        <br />
        <br />
        <button type="button" on:click={handleClick}>Login</button>
    </div>
</main>
