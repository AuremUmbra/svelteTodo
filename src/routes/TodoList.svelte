<script>
    import TodoItem from "./TodoItem.svelte";
<<<<<<< HEAD
=======

>>>>>>> cbba901a3aa28889d184291261ba253994d96932
    export let todoItems;

    $: todosCount = todoItems.length;

<<<<<<< HEAD
    
</script>



=======
</script>

>>>>>>> cbba901a3aa28889d184291261ba253994d96932
Number of todos: { todosCount }
<div class="todo-items">
    {#each todoItems as item}
        <TodoItem {...item} />
    {/each}

</div>

<style>
    .todo-items {
        border: 3px solid
    }
</style>