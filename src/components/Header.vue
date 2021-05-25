<template>
    <header>
        <div>
            <h1>Task Tracker</h1>
            <h2>{{ title }}</h2>
        </div>
        <Button text="Add Task" color="Green"/>
        <Button text="Update task" color="Orange"/>
        <Button text="Remove task" color="Red"/>
        
    </header>
</template>

<script>
import Button from './Button'

export default {
    name: 'Header',
    components: {
        Button,
    },
    props: {
        title: { 
            type: String,
            default: 'Guess',
        },
    },
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
        }

</style>