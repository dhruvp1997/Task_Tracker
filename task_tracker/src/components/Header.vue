<template>
    <header>
        <h1>{{title}}</h1>
        <Button @btn-click="$emit('toggle-add-task')" :text="showAddTask ? 'Close': 'Add Task'" 
        :color="showAddTask ? 'red' : 'green'" />
        
    </header>
</template>
<!-- <Button text="Update Task" color="blue" />
     <Button text="Delete Task" color="red" /> -->
<script>
import Button from './Button'
    export default {
        name: 'Header',
        props: {
            title: String,
            showAddTask: Boolean
            // title: {
            //     type: String,
            //     default: 'Hello World',
            // }
        },
        components: {
            Button
        }
    }
</script>

<style>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>