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
                        <a class="nav-link active" aria-current="page" href="#">{{ page }}</a>
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
                pages: ['Home', 'Location', 'Contact us']
            }
        }
    }
</script>