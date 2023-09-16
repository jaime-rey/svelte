<script>
    let age = 30;
    let name = "Dom"
    let greeting = "";
    $: {
        greeting = `Your name is ${name} and your age is ${age}`
        console.log( `Your name is ${name} and your age is ${age}`)
    }
    function handleClick(){
        ++age;
    }
</script>

<style>

</style>

<p>
    {greeting}
</p>
<button on:click={handleClick}>Increase Age</button>