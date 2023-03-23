<script>
    export let completed;
    export let text;
</script>

<div>
    <input type="checkbox" bind:checked={completed}/> 
    { text }
</div>