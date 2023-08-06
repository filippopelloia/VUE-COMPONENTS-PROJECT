<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Navbar</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" :key="index" id="navbarNav">
                <ul class="navbar-nav">
                    <li v-for="(page, index) in pages" class="nav-item">

                        <a class="nav-link active" 
                           aria-current="page" 
                           :href="page.voice.url"
                        >{{ page.voice.name }}</a>
                        
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        data(){
            return{
                pages: [
                    {
                        voice: {name: 'Home', url: 'home.html'},
                        content: 'This is the end of the world! Enjoy it!'
                    },
                    {
                        voice: {name: 'Location', url: 'location.html'},
                        content: 'Omni-man is currently on the road to the Earth.'
                    },
                    {
                        voice: {name: 'Contacts', url: 'contacts.html'},
                        content: 'It\'s done.'
                    }
                ]
            }
        }
    }
</script>