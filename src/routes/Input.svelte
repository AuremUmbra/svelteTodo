<script>
    import {createEventDispatcher} from "svelte";

    const dispatch = createEventDispatcher();

    let newItemName = "";

    function handleAddClick(event){
        if (newItemName.length === 0) return;
        dispatch("newitem",{newItemName});
        newItemName="";
    }
    
</script>

<div>
    <input type="text" bind:value={newItemName} placeholder="+Add Item"/> <button on:click={handleAddClick} class="button">Add</button>
</div>