<template>
    <section class="header">
        <div class="container">
            <div class="row">
                <div class="col-lg-2 text-right">
                    <img alt="Vue logo" src="../assets/mufachir.jpg" style="width: 150px; height: 150px; border-radius: 50%">           
                </div>
                <div class="col-lg-10 text-left  mt-4">
                    <h1>{{myName}}</h1>
                    <p>{{tagline}}</p>
                </div>
            </div>
        </div>
        <hr/>
    </section>
</template>

<script>

export default ({
    props: {
        myName: {
            type: String,
            required: true
        }, 
        tagline: {
            type: String,
            required: true
        }
    }
})
</script>
