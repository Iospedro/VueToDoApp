<template>
    <div class="home pa-0">
        <field-add-task />
        <list-tasks v-if="$store.state.tasks.length" />
        <no-tasks v-else />

    </div>
</template>
  
<script>
import FieldAddTask from '@/components/Todo/FieldAddTask.vue'
import ListTasks from '@/components/Todo/ListTasks.vue'
import NoTasks from '@/components/Todo/NoTasks.vue'

export default {
    name: 'TodoView',
    components: {
        'field-add-task': FieldAddTask,
        'list-tasks': ListTasks,
        'no-tasks': NoTasks
    }
}
</script>
  