<template>
  <div class="hello">
    <div>{{msg}}</div>
  </div>
</template>

<script>
import abc from './abc';
import skeleton from '../skeleton/Skeleton.vue';
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'xxxxxxxx',
      abc: 'abc',
      obj:{
        a:"ccc"
      },
      arr:["x","c","d"]
    }
  },
  methods:{
    parantFn(pp){
      this.abc = pp;
      console.log("父组件。。。");
    },
    clickFn(){
      this.abc = "zhangzhicheng";
      this.obj.bbbb = "bbb";
      this.arr[5]="555";
      let a="aa";
      let obj={
        [a]:"xxx"
      };
    },
    testFn(a,b,c,d,e){
    }
  },
  computed:{

  },
  components:{
    abc
  },
  created(){

  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang='less'>
.hello /deep/ ul{
    list-style-type: none;
    padding: 0;
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
}
.hello{
  h1, h2 {
    font-weight: normal;
  }
}
</style>
