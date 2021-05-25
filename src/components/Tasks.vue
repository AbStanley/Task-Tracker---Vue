<template>
    <div :key="task.id" v-for="task in tasks" >
        <!-- Loop trough the array 
        annd show what the task comp says.
        -->
        <Task :task="task" />
    </div>
</template>

<script>
import Task from './Task'

export default {
    name: 'Tasks',
    props: {
        tasks: Array
    },
    components: {
       Task,  
    }
}
</script>