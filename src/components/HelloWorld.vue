<template>
  <div class="hello">
    <CompHeader myName="Md. Mufachir Hossain" v-bind:tagline="msg"/>
    

    <section class="content">
      <div class="container">
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
        <h3>Whats are in my skillset</h3>
        <ul>
          <li v-for="mySkill in mySkills" :key="mySkill">
            {{mySkill.name}}  ({{mySkill.yearOfExperience}} Years)
          </li>
        </ul>
      </div>
    </section>
    

    <CompFooter :socialLinks="socialLinks"/>
  </div>
</template>

<script>
  import CompHeader from './CompHeader.vue';
  import CompFooter from './CompFooter';

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components:{
    CompFooter,
    CompHeader
  },
  data() {
    return {
      socialLinks : [
        {name: "Facebook", link: "https://www.facebook.com/mufachir.page"},
        {name: "Twitter", link: "https://twitter.com/cleancoder85"},
        {name: "Linkedin", link: "https://www.linkedin.com/in/mufachir/"},
        {name: "Fiverr", link: "https://fiverr.com/cleancoder85/"}
      ],
      mySkills : [
        {name: "Grails", yearOfExperience: 9},
        {name: "Oracle SQL", yearOfExperience: 9},
        {name: "PLSQL", yearOfExperience: 9},
        {name: "MySQL", yearOfExperience: 10},
        {name: "PostgreSQL", yearOfExperience: 5},
        {name: "jQuery", yearOfExperience: 9},
        {name: "AJAX", yearOfExperience: 8},
      ]
    }    
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
