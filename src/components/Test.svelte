<script> 
   	import { onMount } from 'svelte';
       let onmountstring = "empty"
       let string = `this string contains some <strong>HTML!!!</strong>`;
    
       onMount(async () => {
        onmountstring = "onMount has been executed"
    });

</script>

<p>{@html string}</p>
<p>{ onmountstring }</p>