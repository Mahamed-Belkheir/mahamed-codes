<template>
<nav class="navbar navbar-expand-md navbar-light mb-3 flex-d flex-row-reverse bg-white sticky-top">
    <div class="container flex-d flex-row-reverse">
        <button type="button" class="navbar-toggler" data-target="#navbarCollapse" data-toggle="collapse">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse flex-d flex-row-reverse" id="navbarCollapse">
            <div class="navbar-nav h-20">
                <a href="/" class="nav-item nav-link text-black">About</a>
                <a href="/" class="nav-item nav-link">Experience</a>
                <a href="/" class="nav-item nav-link">Projects</a>
                <a href="/" class="nav-item nav-link">About</a>
            </div>
        </div>
    </div>
</nav>
</template>

<script lang="ts">
export default {
    
}
</script>


<style scoped>
.navbar-light .navbar-nav .nav-link {
    color: black;
    font-size: 1.7rem;
    font-weight: 200;
    margin-left: 1rem;
}
</style>
