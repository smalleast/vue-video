<template>
  <aside class="dev">
    <button class="button" v-on:click="_click1()">video middle</button>
    <div class="main">
      <VueVideo :source="'http://testimg.zhenbaoart.com//o_1bm4po174p8t1kh21iicdlndgm1fl.mp4'" :position="'middle'" ref="video"></VueVideo>
    </div>
  </aside>
</template>
<script>
  import VueVideo from '../components/video.vue'
  export default {
    data() {
      return {};
    },
    props: {},
    created(){
    },
    methods: {
      _click1(){
        this.$refs.video.open();
      }
    },
    components: {VueVideo}
  };
</script>
<style rel="stylesheet/scss" lang="scss">
  .dev {
    text-align: center;
  }

  .button {
    width: 90%;
    height: 50px;
    line-height: 50px;
    background: #af6430;
    text-align: center;
    border-radius: 5px;
    border: 1px solid #fff;
    margin: 10px auto;
    font-size: 18px;
    color: #fff;
  }

  .main {
    width: 6rem;
    height: 6rem;
    border: 1px solid #f00;
    position: relative;
    margin: .2rem .75rem 2rem .75rem;
    background: #ddd;
  }

</style>

