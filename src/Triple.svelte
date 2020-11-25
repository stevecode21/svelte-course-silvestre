<script>
    export let numero;
    $: numeroTriple = numero * 3;
</script>

<p>{numeroTriple} es el triple de {numero}</p>
