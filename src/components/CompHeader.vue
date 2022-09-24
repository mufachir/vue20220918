<template>
    <section class="header">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <img alt="Vue logo" src="../assets/mufachir.jpg" style="width: 150px; height: 150px; border-radius: 50%">
                    <h1>{{myName}}</h1>
                    <p>{{tagline}}</p>
                    <hr/>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

export default ({
  props:[
    'myName', 'tagline'
  ]
})
</script>
