<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <div ref="ic" @click="clickFn">xhxhxh</div>
    <p>{{abc}}</p> 
    <p>{{obj.bbbb}}</p> 
    <p>{{arr[5]}}</p> 
    <p>{{abc2}}</p> 
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: '子页面',
      abc: 'abc',
      obj:{
        a:"ccc"
      },
      arr:["x","c","d"]
    }
  },
  props:{
    abc2:{
      default:"xxx",
      type: String
    }
  },
  methods:{

    clickFn(){
    },
    testFn(a,b,c,d,e){

    }
  },
  computed:{

  },
  components:{

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
