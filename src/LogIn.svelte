<script>
    let user = { loggedIn: false };

    function toggle() {
       user.loggedIn ^= 1;
    }
</script>

{#if user.loggedIn}
    <button on:click={toggle}>
        Log out
    </button>
{/if}

{#if !user.loggedIn}
    <button on:click={toggle}>
        Log In
    </button>
{/if}