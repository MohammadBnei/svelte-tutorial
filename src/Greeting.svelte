<style>
    h2 {
        color: purple;
        font-family: 'Comic Sans MS';
        font-size: 2em;
    }
</style>

<script>
    export let first_name;
    export let last_name;

    $: name = first_name + " " + last_name;
</script>

<h2>Hello {name}!</h2>