<script>
    import Datos from './Datos.svelte';
    export let name;
    let language = 'Svelte';
    let fullName = {
        name: 'Lola',
        lastName: 'Palsd',
    };
</script>

<h1>Hola {name}</h1>
<Datos {language} {...fullName} />
