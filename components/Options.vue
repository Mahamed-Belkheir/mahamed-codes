<template>
    <div class="col options">
            <div 
            v-for="(value, i) in items"
            :key="value[0]"
            :class="{active: chosen == i}"
            v-on:click="pick(i)"
            class="row pl-sm-auto pr-sm-auto option text-center">
                {{value[0]}}
            </div>
    </div>
</template>


<script lang="ts">
import Vue from "Vue";
export default Vue.extend({
props: {
        items: Array,
        cb: Function
    },
    data: function() {
        return {
            chosen: 0
        }
    },
    methods: {
        pick(i: number) {
            this.chosen = i
            this.cb(i)
        }
    }
})
</script>


<style scoped>
.option {
    justify-content: center;
    font-weight: bold;
    border: 2px solid white;
    width: 30%;
}

.option:hover {
    cursor: pointer;
}


.options {
    justify-content: space-between;
}

@media only screen and (min-width: 600px) {
  .options {
    display: flex;

  }
}


@media only screen and (max-width: 600px) {
  .option {
    width: 111%;
  }
  
}

.active {
    font-weight: bold;
    border: 2px solid;
    border-image-slice: 1;
    border-image-source: linear-gradient(
        to left,
        #2F80ED,
        #6FCF97
    );
    
}
</style>