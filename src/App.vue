<template>
    <div id="app">
        {{title}}
        <Character
        v-for="(id, index) in initial_ids" 
        :id="id"
        :key="index" 
        />  
    </div>
</template>

<script>
import Character from './components/Character.vue'
export default {
    name: 'app',
    data() {
        return {
            title: 'Generate Your team',
            initial_ids: [1, 13, 14]
        }
    },
    components: {
        Character
    }
}
</script>
