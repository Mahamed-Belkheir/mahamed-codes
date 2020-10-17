<template>
    <div class="container">
        <div class="row-12 h-100">
            <div class="col-sm-12 col-md-6">
                <h2>Get in Touch</h2>
            </div>
            <div class="col-sm-12 col-md-12 d-flex flex-column align-items-center h-25 links">
                <a target="_blank" href="https://github.com/Mahamed-Belkheir"> Github </a>
                <a target="_blank" href="https://www.linkedin.com/in/mahamedbelkheir/"> Linkedin </a>
            </div>            
        </div>
    </div>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
})
</script>

<style scoped>

.container {
    margin-top: 6rem;
}

.links {
    margin-top: 7rem;
}

h2 {
    font-weight: 300;
    font-size: 3rem;
    border-bottom: 2px solid;
    border-image-slice: 1;
    border-image-source: linear-gradient(
    to left,
    #2F80ED,
    #6FCF97
    );
    margin-bottom: 1rem;
    padding: 5px;
}

p {
    margin-top: 1rem;
}

a {
    padding: 10px;
    margin: 4px;
    border: 2px solid;
    border-image-slice: 1;
    border-image-source: linear-gradient(
    to left,
    #2F80ED,
    #6FCF97
    );
    width: 35%;
    justify-content: center;
    align-items: center;
    align-content: center;
    text-align: center;
    color: black;
}
</style>