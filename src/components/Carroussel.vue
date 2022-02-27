<template>
    <main class="spaceCarroussel pt-5 pb-5">
            <div class="d-flex justify-content-center">
                <h1 class="titleSection pb-2">
                    {{titleSection}}
                </h1>
            </div>
        <div class="container col-md-12 d-flex justify-content-center pt-5 pb-3">
            <Splide :options="options">
                <SplideSlide class="sliderContent" v-for="carrousselItem in carrousselItems" :key="carrousselItem.id" >
                    <h2 class="d-flex justify-content-center titleCarroussel pb-3">
                        {{carrousselItem.title}}
                    </h2>
                    <p class="text-center">
                        {{carrousselItem.text}}
                    </p>
                </SplideSlide>
            </Splide>
        </div>
    </main>
</template>
<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/splide/dist/css/themes/splide-default.min.css';


export default {
    name: 'Carroussel',
    components:{
        Splide,
        SplideSlide,
    },
    data: () => {
        return{
            options:{
                rewind: true,
                width: 650,
                height: 200,
                padding: '4rem',
                gap: '5rem'
            },
            titleSection: 'Lorem',
            carrousselItems: [
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'},
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'},
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'},
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'},
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'},
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'},
                {title: 'Lorem Ipsum', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius.'}
            ]
        }
    }
}


</script>
<style scoped>
    h2{
        position: relative;
        color: #fff;
    }
    h2::before{
        content: "";
        width: 100px;
        height: 2px;
        background-color: #fff;
        position: absolute;
        opacity: .5;
        top: 50px;
        border-radius: 1rem;
    }
    p{
        color: #fff;
        font-size: 14pt;
    }
    .titleSection{
        color: white;
        display: flex;
        justify-content: center;
        position: relative;
        font-size: 40pt;
    }
    .spaceCarroussel{
        background: rgb(154,29,162);
        background: linear-gradient(45deg, rgba(154,29,162,1) 32%, rgba(0,212,255,1) 100%);
        box-shadow: 0 0 20px grey;
    }
</style>