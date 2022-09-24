<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      I am a passionate software engineer, entreprenuer. <br/>
      I love to learn new things, read books, serve people. <br/>
      This time I am learning Vue.js and creating my personal website.
    </p>
    <h3>Projects I've worked on so far...</h3>
    <ul>
      <li>
        <a href="https://erp.aub.edu.bd" target="_blank" rel="noopener">SUERP for AUB</a>
      </li>
      <li><a href="https://admission.aub.edu.bd" target="_blank" rel="noopener">Online Admission for AUB</a></li>
      <li><a href="https://myasian.aub.edu.bd" target="_blank" rel="noopener">MyAsian</a></li>
      <li><a href="https://softrithmit.com/newsdetail/news/2021-01-07-payment-through-softrithm-bank-api-has-been-launched-for-aub-students"  rel="noopener">Bank Payment API for AUB (SEBL, SIBL, AIBL)</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    

    <CompFooter/>
  </div>
</template>

<script>
  import CompFooter from './CompFooter';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components:{
    CompFooter
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
</style>
