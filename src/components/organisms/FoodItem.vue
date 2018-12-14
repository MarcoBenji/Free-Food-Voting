<template>
    <div>
        <div class="top">
            <Title class=title 
                title="first food item">
            </Title>
            <p class=datetime> {{DateAndTime}} </p>
        </div>
        <div class="mid">
            <UpAndDownVoting class=voting> </UpAndDownVoting>
            <TextBox class=description
                content="YEY IT WAS FOOD!!!!"> 
            </TextBox>
        </div>
        <div class="button">
            <button type="button">Comment</button>
        </div>
    </div>
</template>



<script>
    import Title from '../atom/Title';
    import TextBox from '../atom/TextBox';
    import UpAndDownVoting from '../molecules/UpAndDownVoting';

    export default {
        name: 'FoodItem',
        components: {
            Title,
            TextBox,
            UpAndDownVoting
        },
        props: {
            DateAndTime: {
                // type: String,
                required: true
            }
        },
        computed: {
            foodUrl() {
                return `url(http://calm-caverns-24814.herokuapp.com/food)`;
            }
        }
    }
  
    
</script>

<style scoped>
    .top {
        display: flex;
        justify-content: space-between;
        text-align: center;
        width: 95%;
        margin: auto;
    }
    .mid {
        
    }
    .button {
        text-align: right;
        width: 100%;
        padding-right: 10px;
        padding-bottom:5px;
    }
</style>