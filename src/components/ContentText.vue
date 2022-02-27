<template>
    <div class="container pt-5 pb-5">
        <div class="row">
            <div class="col-md-6">
                <div v-for="textItem in textItems" :key="textItem.id" class="text1 pt-3">
                    <h4>
                        {{textItem.titleText}}
                    </h4>
                    <p class="text-justify">
                        {{textItem.text}}
                    </p>
                </div>
            </div>
            <div class="col-md-6">
                <div v-for="textItem in textItems" :key="textItem.id" class="text1 pt-3">
                    <h4>
                        {{textItem.titleText}}
                    </h4>
                    <p class="text-justify">
                        {{textItem.text}}
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>

</style>
<script>
export default {
    name: 'ContentText',
    data:() => {
        return{
            textItems: [
                {titleText: 'Lorem ipsum dolor sit amet',
                text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius. Nulla vitae dui nec mauris placerat sollicitudin elementum eget leo. Ut eget neque nulla. Nunc semper velit at magna ultrices, a facilisis massa porta. Donec sed lacus nec elit bibendum finibus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Sed vestibulum tempor euismod.'},
                {titleText: 'Lorem ipsum dolor sit amet',
                text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius. Nulla vitae dui nec mauris placerat sollicitudin elementum eget leo. Ut eget neque nulla. Nunc semper velit at magna ultrices, a facilisis massa porta. Donec sed lacus nec elit bibendum finibus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Sed vestibulum tempor euismod.'},
                {titleText: 'Lorem ipsum dolor sit amet',
                text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis tortor at nisi cursus, ut egestas leo vestibulum. Nullam et ante et sapien semper varius. Nulla vitae dui nec mauris placerat sollicitudin elementum eget leo. Ut eget neque nulla. Nunc semper velit at magna ultrices, a facilisis massa porta. Donec sed lacus nec elit bibendum finibus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Sed vestibulum tempor euismod.'}
            ]
        }
    }
}
</script>