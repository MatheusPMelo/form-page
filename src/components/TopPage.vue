<template>
    <div class="mainTopPage container">
        <div class="row pt-3">
            <div class="logo col-md-6 col-6">
                <a href="">
                    <img 
                    src="./../assets/logo.png"
                    alt=""
                    class="img-fluid"
                    >
                </a>
            </div>
            <div class="col-md-6 col-6 d-flex justify-content-end align-items-center">
                <button class="btn">{{btn}}</button>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .logo a img{
        width: 150px;
    }

    .btn {
        box-sizing: border-box;
            -webkit-appearance: none;
            -moz-appearance: none;
        appearance: none;
        background-color: transparent;
        border: 2px solid #000623;
        border-radius: 0.6em;
        color: #000623;
        cursor: pointer;
        display: -webkit-box;
        display: -webkit-flex;
        display: -ms-flexbox;
        display: flex;
        -webkit-align-self: center;
            -ms-flex-item-align: center;
                align-self: center;
        font-size: 12pt;
        font-weight: 400;
        line-height: 1;
        margin: 20px;
        padding: 1.2em 2.8em;
        text-decoration: none;
        text-align: center;
        font-family: 'Montserrat', sans-serif;
        font-weight: 700;
    }
    .btn:hover, .btn:focus {
      color: #fff;
      outline: none;
    }

    button{
        color: #fff;
        box-shadow: 0 0 40px 40px #ffffff10 inset, 0 0 0 0 #ffffff;
        -webkit-transition: all 150ms ease-in-out;
        transition: all 150ms ease-in-out;
        backdrop-filter: blur(10px);
    }
    button:hover{
        border: 2px solid #32b3ec;
        box-shadow: 0 0 10px 0 #32b3ec inset, 0 0 0 2px#32b3ec;
        backdrop-filter: blur(100px);
    }
    button:focus{
        outline: none;
    }
    button:active{
        background-color: #1c2c48;
    }
</style>

<script>
export default {
    name: 'TopPage',
    props: {
        'btn': String
    }
}
</script>