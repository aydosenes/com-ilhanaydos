<template>
    <div class="carousel">
        <slot></slot>
        <button @click.prevent="next" class="next">❯</button>
        <button @click.prevent="prev" class="prev">❮</button>
    </div>
</template>
<script>
export default {
    data () {
        return {
            index : 0,
            slides : [],
            slideDirection: "",
        }
    },
    // mounted(){
    //     this.slides = this.$children;
    //     this.slides.map( (slide,index) => {
    //         slide.index = index;
    //     });
    // },
    methods: {
        next() {
            this.$emit("next")
        },
        prev() {
            this.$emit("prev")
        }
    }
}
</script>
<style>
    .carousel {
        position: relative;
        width: 600px;
        height: 350px;
        overflow: hidden;
    }
    button {
        position: absolute;
        width: 50px;
        height: 40px;
        top: calc(50% - 20px);
        background-color: rgba(173, 173, 173, 0.8);
        border: none;
        color: #FFF;        
    }
    button:focus, button:hover {
        outline: none;
        cursor: pointer;
    }
    .next {
        right: 0;
    }
    .prev {
        left: 0;
    }

</style>