<script>
    $: console.log('hello');
    $: {
        // expression
    }

    $: if (argument) {
        // return
    } else {
        // return;
    }

    $: for (let index = 0; index < Array.length; index++) {
        const element = array[index];
    }

    $: variable = argument => {
        //return
    };

    $: async () => {
        bar = await Promise.resolve(argument);
    };

    $: ({ a, b } = object);
</script>
