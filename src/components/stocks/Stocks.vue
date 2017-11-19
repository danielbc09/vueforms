<template>
    <div>
        <app-stock v-for="stock in stocks"></app-stock>
    </div>
</template>
<script>
    import Stock from './Stock.vue';
    export default {
        data(){
            return{
                stocks:[
                    {id:1, name:'BMW', price:100},
                    {id:1, name:'Google', price:200},
                    {id:1, name:'Apple', price:300},
                    {id:1, name:'Twitter', price:10},
                ]
            }
        },
        components:{
            'app-stock': Stock,
        }
    }
</script>