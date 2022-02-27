<template>
    <div class="footer container pt-5 pb-5 d-flex">
        <div class="col-md-6 col-6">
            <div class="d-flex justify-content-start">
                <a href="#">
                    <img 
                        src="./../assets/logo.png"
                        class="img-fluid"
                    >
                </a>
            </div>
        </div>
        <div class="col-md-6 col-6 d-flex justify-content-end align-items-end">
            <div class="">
                <p>{{text}}</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Footer',
    data: () => {
        return{
            text: 'Site criado por Matheus Melo'
        }
    }
}
</script>
<style scoped>
    
</style>