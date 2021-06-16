<template>
    <header>
        <h1>{{title}}</h1>
        <Button text="Add Task" color="green" />
        
    </header>
</template>
<!-- <Button text="Update Task" color="blue" />
     <Button text="Delete Task" color="red" /> -->
<script>
import Button from './Button'
    export default {
        name: 'Header',
        props: {
            title: String
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