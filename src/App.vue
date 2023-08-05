<template>
    <p>Simple text</p>
    <h1>{{ marando }}</h1>
</template>

<script>
    import PageViewer from './components/PageViewer.vue';
    import Navbar from './components/Navbar.vue';

    export default {
        components: {    //UTILE PER RACCHIUDERE LE COMP CHE CI SERVONO
            Navbar,
            PageViewer,
        },
        data() {
            return {
                marando: 'Io me ciamo Luigi Marando!!'
            }
        }
    }
</script>