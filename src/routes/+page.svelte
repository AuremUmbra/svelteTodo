<script>
    import Input from './Input.svelte';
    import TodoList from './TodoList.svelte';

    let newItemName;

    let todoItems = [
        {"completed": false, "text": "Learn Svelte"}, // 0
        {"completed": false, "text": "Make Toast"},    // 1
        {"completed": true, "text": "Make Coffee"}
    ];

    function handleNewItem(event){
        newItemName = event.detail.newItemName;
        todoItems=[...todoItems,{"completed": false,"text": newItemName}]
    };
</script>

<h1>Todo App Class Activity</h1>

<Input on:newitem={handleNewItem} />

<TodoList todoItems={todoItems}/>

