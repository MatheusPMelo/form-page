<template>
    <div class="container">
        <div class="title col-md-12 d-flex justify-content-center">
            <h1>{{mainTitle}}</h1>
        </div>
        <div class="subTitle col-md-12 d-flex justify-content-center">
            <h3>{{subTitle}}</h3>
        </div>
    </div>
</template>

<style scoped>
*{
    color:white
}
h3{
    font-weight: 100;
    opacity: .5;
    position: relative;
    display: flex;
    justify-content: center;
}
h3::before{
    content: "";
    position: absolute;
    width: 30vh;
    height: 2px;
    background-color: white;
    border-radius: 1rem;
    display: flex;
    top: 50px;
    box-shadow: 0 0 5px #fff;
}
</style>

<script>
export default {
    name: 'Title',
    props:{
        'mainTitle': String,
        'subTitle': String
    }
}
</script>