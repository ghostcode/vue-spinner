<template>
    <div>
    
    </div>
</template>
<script>
import Spinner from './spin.js'

export default {
    name: 'spinner',
    props: {
        lines: { type: Number, default: 12 }, // The number of lines to draw
        length: { type: Number, default: 10 }, // The length of each line
        width: { type: Number, default: 14 }, // The line thickness
        radius: { type: Number, default: 42 }, // The radius of the inner circle
        scale: { type: Number, default: 1 }, // Scales overall size of the spinner
        corners: { type: Number, default: 1 }, // Corner roundness (0..1)
        color: { type: String, default: '#000' }, // #rgb or #rrggbb or array of colors
        opacity: { type: Number, default: 0 }, // Opacity of the lines
        rotate: { type: Number, default: 0 }, // The rotation offset
        direction: { type: Number, default: 1 }, // 1: clockwise, -1: counterclockwise
        speed: { type: Number, default: 1 }, // Rounds per second
        trail: { type: Number, default: 60 }, // Afterglow percentage
        fps: { type: Number, default: 20 }, // Frames per second when using setTimeout() as a fallback for CSS
        zIndex: { type: Number, default: 1000 }, // The z-index (defaults to 2000000000)
        className: { type: Number, default: 'spinner' }, // The CSS class to assign to the spinner
        top: { type: String, default: '50%' }, // Top position relative to parent
        left: { type: String, default: '50%' }, // Left position relative to parent
        shadow: { type: Boolean, default: false }, // Whether to render a shadow
        hwaccel: { type: Boolean, default: false }, // Whether to use hardware acceleration
        position: { type: String, default: 'absolute' } // Element positioning

    },
    // ready(){
    mounted() {
        let self = this

        let {
            lines,
            length,
            width,
            radius,
            scale,
            corners,
            color,
            opacity,
            rotate,
            direction,
            speed,
            trail,
            fps,
            zIndex,
            className,
            top,
            left,
            shadow,
            hwaccel,
            position
        } = this

        self.spinner = new Spinner({
            lines,
            length,
            width,
            radius,
            scale,
            corners,
            color,
            opacity,
            rotate,
            direction,
            speed,
            trail,
            fps,
            zIndex,
            className,
            top,
            left,
            shadow,
            hwaccel,
            position
        }).spin(self.$el)
    }
}
</script>
<style>

</style>


