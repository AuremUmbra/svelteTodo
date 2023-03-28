<script>
    import Input from './Input.svelte';
    import TodoList from './TodoList.svelte';

<<<<<<< HEAD
    let newItemName;

=======
>>>>>>> cbba901a3aa28889d184291261ba253994d96932
    let todoItems = [
        {"completed": false, "text": "Learn Svelte"}, // 0
        {"completed": false, "text": "Make Toast"},    // 1
        {"completed": true, "text": "Make Coffee"}
<<<<<<< HEAD
    ];

    function handleNewItem(event){
        newItemName = event.detail.newItemName;
        todoItems=[...todoItems,{"completed": false,"text": newItemName}]
    };
=======
    ]

    let newItemName;

    function handleNewItem(event) {
        newItemName = event.detail.name;
        addNewItem();
    }

    function addNewItem() {
        let newItem  = {"completed": false, "text": newItemName};
        todoItems = [...todoItems, newItem]
    }
>>>>>>> cbba901a3aa28889d184291261ba253994d96932
</script>

<h1>Todo App Class Activity</h1>

<<<<<<< HEAD
<Input on:newitem={handleNewItem} />

<TodoList todoItems={todoItems}/>
=======
<Input on:newItem={handleNewItem}/>

<TodoList todoItems={todoItems} />
>>>>>>> cbba901a3aa28889d184291261ba253994d96932

