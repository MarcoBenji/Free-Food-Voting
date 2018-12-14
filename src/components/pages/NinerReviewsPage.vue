<template>
    <div class=page>
        <div class=header>
            <span>Add Food</span>
            <h1>Free 9er Food Feedback</h1>
        </div>
        <div>
            <div class=row>
                <FoodItem v-bind:DateAndTime="new Date()">
                    
                </FoodItem>
            </div>
        </div>
    </div>
</template>

<script>
    import FoodItem from '../organisms/FoodItem';

    export default {
        name: 'NinerReviewsPage',
        components: {
            FoodItem
        }
    }
</script>

<style scoped>
    .header {
        display: flex;
        justify-content: space-between;
        text-align: center;
    }
    .row {
        width: 75%;
        margin: auto;
        border: 3px solid black;
        position: relative;
    }
</style>