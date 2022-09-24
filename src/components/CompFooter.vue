<template>
    <section class="footer">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    Find me on: 
                    <ul>
                        <li v-for="socialLink in socialLinks" :key="socialLink">
                            <a  :href="socialLink.link">
                                {{socialLink.name}}
                            </a> 
                        </li>                        
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default({
   props:{
        socialLinks: {
            type: Array
        }
   }
})
</script>


<style scoped>
  .footer{
    background-color: black;
    padding: 20px 0;
    font-size: 2em;
  }
  ul {
    list-style-type: none;
  }
  ul li{
    display: inline;
    margin: 5px;
  }
</style>