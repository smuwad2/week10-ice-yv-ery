<script>
    //import component
    import SoundIcon from './subcomponents/SoundIcon.vue'
    export default { 
        data() {
            return {
                soundLevel: 0
            }
        },
        components: {
            SoundIcon
        }
    }
</script>

<template>

   Sound level
    <input type="number" min="0" max="3" v-model="soundLevel"> 
    <!-- TODO: Add Code Here to make use of the component -->
    <sound-icon :level="soundLevel"></sound-icon> <!-- Since its a dynamic var, need to put the : before the level but if its a static value then no need -->
    

</template>

