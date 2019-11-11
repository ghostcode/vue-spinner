# vue-simple-spin

spin for Vue 2/1 (At the beginning,I want to name it vue-spinner but it's already used and also vue-simple-spinner,so I call it vue-simple-sin)

# Preview

![WX20191111-113527](https://user-images.githubusercontent.com/745181/68559274-5f04f080-0477-11ea-855f-d554436077a8.png)


# Usage

Install:

    npm i -S vue-simple-spin

Import:

    <template>
        <spinner></spinner>
    </template>

    <script>
    import Spinner from 'vue-simple-spin'

    export default {
        components: {
            Spinner
        }
    }
    </script>

# Settings

    var opts = {
        lines: 13 // The number of lines to draw
        , length: 28 // The length of each line
        , width: 14 // The line thickness
        , radius: 42 // The radius of the inner circle
        , scale: 1 // Scales overall size of the spinner
        , corners: 1 // Corner roundness (0..1)
        , color: '#000' // #rgb or #rrggbb or array of colors
        , opacity: 0.25 // Opacity of the lines
        , rotate: 0 // The rotation offset
        , direction: 1 // 1: clockwise, -1: counterclockwise
        , speed: 1 // Rounds per second
        , trail: 60 // Afterglow percentage
        , fps: 20 // Frames per second when using setTimeout() as a fallback for CSS
        , zIndex: 2e9 // The z-index (defaults to 2000000000)
        , className: 'spinner' // The CSS class to assign to the spinner
        , top: '50%' // Top position relative to parent
        , left: '50%' // Left position relative to parent
        , shadow: false // Whether to render a shadow
        , hwaccel: false // Whether to use hardware acceleration
        , position: 'absolute' // Element positioning
    }

# Thanks

Depend on Felix Gnass's [spin](https://github.com/fgnass/spin.js)
