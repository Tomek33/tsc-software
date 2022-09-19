<template>
    <div>
        <div class="row my-background-green">
            <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Header></Header>
            </div>
            <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Row1 :isLargeScreen="isLargeScreen"></Row1>
            </div>
        </div>

        <div class="row">
          <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Row2></Row2>
            </div>
        </div>

        <div class="row my-5">
          <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Row3></Row3>
            </div>
        </div>

        <div class="row my-5">
          <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Row4 :isLargeScreen="isLargeScreen"></Row4>
            </div>
        </div>

        <div class="row my-5">
          <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Row5></Row5>
            </div>
        </div>

        <div class="row my-5 my-background-green">
          <div v-bind:class="{ 'ps-5': isLargeScreen, 'pe-5': isLargeScreen }">
                <Footer  :isLargeScreen="isLargeScreen"></Footer>
            </div>
        </div>
      
    </div>
</template>

<style scoped>
    .my-background-green{
        background-color: #74C69D;
    }
</style>

<script>
    import Header from './Header.vue'
    import Row1 from './Row1.vue'
    import Row2 from './Row2.vue'
    import Row3 from './Row3.vue'
    import Row4 from './Row4.vue'
    import Row5 from './Row5.vue'
    import Footer from './Footer.vue'
    
    export default {
    name: "Layout",
    components: { Header, Row1, Row2, Row3, Row4, Row5, Footer },
    data() {
        return {
            windowWidth: window.innerWidth
        }
    },
    mounted() {
    this.$nextTick(() => {
      window.addEventListener('resize', this.onResize);
    })
  },
  beforeDestroy() { 
    window.removeEventListener('resize', this.onResize); 
  },
  computed:{
    isLargeScreen(){
        return this.windowWidth > 575;
    }
  },
  methods: {  
    onResize() {
      this.windowWidth = window.innerWidth
    }
  }
}
</script>