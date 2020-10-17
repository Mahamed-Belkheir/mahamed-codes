<template>
<div class="container-fluid app">
    <Navbar />
    <div class="col-md-12 h-100">
        <div class="row h-25"  id="about">
            <About/>
        </div>
        <div class="row h-25" id="experience">
            <Experience/>
        </div>
        <div class="row h-25" id="projects">
            <Projects/>
        </div>
        <div class="row h-25" id="contact">
            <About/>
        </div>
    </div>
</div>
</template>


<style>
.app {
    height: 400vh;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Poppins';
}

</style>