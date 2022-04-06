<script>
    import Button from "@smui/button"
    import Textfield from "@smui/textfield"
    
    let client = {
        name: "",
        firtsName: "",
        cpf: ""
    }
</script>


<Textfield variant="filled" bind:value={client.name} label="Nome"/>
<Textfield variant="filled" bind:value={client.firtsName} label="Sobrenome"/>
<Textfield variant="filled" bind:value={client.cpf} label="Cpf"/>

<Button variant="raised"> Salvar </Button>

<p>{client.name}</p>
<p>{client.firtsName}</p>
<p>{client.cpf}</p>