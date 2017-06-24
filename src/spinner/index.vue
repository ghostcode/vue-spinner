<template>
    <div>
    
    </div>
</template>
<script>
import Spinner from './spin.js'

export default {
    name: 'spinner',
    // ready(){
    mounted() {
        let self = this
        self.spinner = new Spinner({
            color: '#42b983',
            lines: 12
        }).spin(self.$el)
    }
}
</script>
<style>

</style>


