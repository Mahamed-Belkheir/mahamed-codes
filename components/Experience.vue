<template>
    <div class="container">
        <div class="row-12 h-100">
            <div class="col-sm-12 col-md-6">
                <h2>Experience</h2>
            </div>
            <div class="col-sm-12 col-md-6">
                <Options :items="experiences" :cb="publish" />
            </div>            
            
            <div class="col-sm-12 col-md-6">
                <p>{{text}}</p>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
export default {

    data: function() {
       return {
            experiences: [
            ["Inspectron", "Lorem one ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex."],
            ["Ion Tele & Tech", "Lorem two ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex."],
            ["RBK", "Lorem three ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex."],
            ],
           
            text: ""
        }
    },
    methods: {
           publish(i: number) {
               this.text = this.experiences[i][1]
           }
    },
    mounted() {
        this.text = this.experiences[0][1]
    }
}
</script>

<style scoped>
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
</style>