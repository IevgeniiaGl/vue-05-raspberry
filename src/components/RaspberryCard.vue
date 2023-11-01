
<template>
    <div class='card'>
        <div class="image"><img :src="cardData.imgSrc" ></div>
        <div class='block'>
                <div class="logo"><img :src="cardData.logo"></div>
                <div class="title">{{cardData.companyTitle}}</div>
        </div>
         <div class="description">{{cardData.description}}</div>
       
    </div>
</template>

<script>
    export default {
        name:'RaspberryCard',

        props:{
            cardData:{
                type:Object,
                default:()=>({})
            }
        }
    }
</script>

<style lang="css" scoped>
.card {
    color: #ffffff;
    }



		.image img{
            width: 200px;
            height: 170px;
            border-radius: 10px;
           
		}

		.logo {
		}

        .block {
         display: flex;
         gap: 10px;
        

		}



		.company-title {
            
		}



		.description {
            text-align: left;
		}



</style>