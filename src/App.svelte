<script>
    import Datos from './Datos.svelte';
    import Button from './Button.svelte';
    import Triple from './Triple.svelte';
    export let name;
    let language = 'Svelte';
    let fullName = {
        name: 'Lola',
        lastName: 'Palsd',
    };
    let disabled = true;
    let numero = 0;
    function handleClick() {
        numero += 1;
    }

    $: numeroDoble = numero * 2;
</script>

<h1>Hola {name}</h1>
<Datos {language} {...fullName} />
<Button {disabled} />
<button on:click={handleClick}>{numero}</button>
<p>{numeroDoble} es el doble de {numero}</p>
<Triple {numero} />
