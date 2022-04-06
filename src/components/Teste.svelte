<script>
    export let name = "Augusto Peçanha"
    let number = 0
    $: numberQ = number * number
    $: {if(numberQ > 100){
        alert(`O valor ${numberQ} é maior que 100`)
    }}
</script>


<h1>
    {`${name} ${number}`}
</h1>

<button on:click={() => number++}> + </button>
<button on:click={() => number--}> - </button>

<p>
    {@html "<strong> Teste </strong>"} {numberQ}
</p>

<style>
    h1{
        color: brown;
    }

</style>