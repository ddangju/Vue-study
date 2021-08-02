<template>

<div>
  <div class="menu">
    
    <a v-for="(name,i) in menu" :key="name">{{i}}{{name}}</a>
  </div>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>

  <div v-for="(title,i) in 3" :key="i">
    <h4>{{products[i]}}</h4>
    <p>50마넌</p>
  </div>
  <!-- <div>
    <h4>{{products[0]}}</h4>
    <p>만원</p> -->
    <!-- <App-header :messege="propsdata" :textData="text" :productData="products"/>
    {{messege}} -->
  <!-- </div>
  <div>
    <h4>{{products[1]}}</h4>
    <p>천원</p>
  </div>
  <div>
    <h4>{{products[2]}}</h4>
    <p>천원</p>
  </div> -->
  <!-- <input class="abc" v-model="text" type="text" />
  {{text}} -->
  <!-- <button class="btn" @click="[btnClick(),change()]"> 버튼 </button>
  <div class="list"> -->
    <!-- {{this.products}} -->
    <!-- {{products}}
  </div> -->
  <!-- <div>
    <input class="def" type="text" placeholder="hi"/>
  </div> -->
  <!-- <div class="box" :blocklist="block"></div>
  <button class="btn" @click="handleClick"> 추가하기 </button> -->
  
</div>
</template>

<script>
// import AppHeader from '@/components/App-header.vue'
// @ is an alias to /src

export default {
  name: 'Home',
  data(){
    return{
      text: "",
      products :['역삼동원룸', '천혼동원룸', '마포구원룸'],
      menu:['home', 'products', 'about'],
      price:['만원', '오천원', '천원'],
      block: [],
      // style: 'color : blue',
    }
  },
  components: {
    // AppHeader
    
  },
  methods: {
    btnClick(){
      this.products.push(this.text,)
    },
    change(){
      this.text = ""
    },
    handleClick() {
      this.block.push(this.block)
      
    },
  },
  // props:{
  //   propsdata:"hi"
  // }
}
</script>

<style lang="scss">

.menu{
  background-color:rgb(12, 63, 56);
  font-size:20px;
  padding: 15px;
  border-radius: 5px;
  a{
    color:white;
    font-size:25px;
    margin-right:50px;
    font-weight: 700;
    padding:10px;
  }
}

</style>