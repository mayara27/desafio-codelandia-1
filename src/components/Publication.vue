<template>
   <div >
       <div class="card" v-for="(pub) in pubs" :key="pub.title">
           <p class="date"> {{ pub.date }} </p>
            <v-icon class="icon-heart"
            color="#574AE8">
            mdi-heart-outline
            </v-icon>
            <h2 class="card-title"> {{ pub.title }} </h2>
            <p class="card-body"> {{ pub.body }} </p>
       </div>
    </div>
</template>

<script>
export default {
    props: {
        pubs: { type: Array, required: true }
    },
}
</script>

<style>
    .card {
        position: relative;
        width: 70%;
        min-height: 150px;
        left: 15%;
        background: #FFFFFF;
        box-shadow: 0px 0px 10px rgba(19, 19, 31, 0.05);
        border-radius: 5px;
        color: black;
        margin-bottom: 50px;
        padding: 30px;
    }

    .date {
        color: #B6B6B6;
        display: inline-block;
        padding-bottom: 20px;
    }

    .card-title {
        font-weight: normal;
        margin-bottom: 15px;
        color: #313131;
    }

    .card-body {
        line-height: 32px;
        color: #B6B6B6;
        font-family: Lexend Deca;
        font-weight: normal;
        font-size: 18px;
    }
    .icon-heart {
        float: right;
    }

</style>