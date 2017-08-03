#vue-video
> video for vue.

## props:

```
 props: {
           source: {
             type: String,
             default: ''
           },
           position: {
             type: String,
             default: 'middle'
           }
    },
```

## usage:
+ install:
```bash
npm install smalleast/vue-video --save


```

+ code:
```javascript
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

```

+template
```
<template>
  <aside class="dev">
    <button class="button" v-on:click="_click1()">video middle</button>
    <div class="main">
      <VueVideo :source="'http://testimg.zhenbaoart.com//o_1bm4po174p8t1kh21iicdlndgm1fl.mp4'" :position="'middle'" ref="video"></VueVideo>
    </div>
  </aside>
</template>
```

## resource:
+ http://www.cnblogs.com/Kummy/p/4966937.html
+ https://github.com/steven5538/vue-button
+ https://yarnpkg.com/en/docs/install
