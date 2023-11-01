<template>
    <div class='panel'>
<raspberry-card v-for="card in cardsListData" 
                :key="card.id"
                :card-data="card"
                
            />
    </div>
</template>

<script>
import RaspberryCard from './RaspberryCard.vue'




    export default {
        name:'RaspberryPanel',
        components:{  RaspberryCard},
        props:{
            cardsListData:{
              type:Array,
              default:() => [],
            }
        }
    }
</script>

<style lang="css" scoped>
.panel{
    background: #292929;
    display: flex;
    gap: 20px;
    align-items: center;
    justify-content: center;
    padding: 30px;
}
   

</style>