<script>
    // TODO: Add other states for the application
    let username = "USER";

    function handleClick() {
        if(document.getElementById("pass").value=="bhavani")
        alert("Congratulations!!! You have found the password")
        else
        alert("Sorry ! You've not found the password , Try again !")
    }
</script>

<style>
    /* TODO: Add Styles to application  */
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
        transform: translate(0%,50%);
       box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
       width: 35%;
       height:45%;
       background-color:#d1d8e0;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
    .right{
        float: right;
        transform: translate(0%,-60%);
    }
    .left{
        transform: translateX(-20%);
    }
    .clue{
        transform: translateY(17%);
    }
</style>
<main>
    
    <br>
    <div class="left">
        <h2>Find the Password !</h2>
        <br>
        <input type="text" placeholder="Username" bind:value={username} readonly/>
        <br>
        <input type="password" id="pass" placeholder="Enter the password" />
    </div>
    <div class="right">
        <img src="/bhavani.jpeg" alt="" height="310px" class="clue">
        <br><br><br>
        <h3>CLUE</h3>
    </div>
    <br>
        <button on:click={handleClick}>Login !</button>
</main>