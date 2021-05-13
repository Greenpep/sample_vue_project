<template>
    <div class="block" @click="applauseOnce">
        click to applause
    </div>
    <p> Applause Counter: {{ applause_counter }} </p>
</template>

<script>
export default {
    props: ['applause_counter'],
    methods: {
        applauseOnce(){
            applause_counter++
        }
    }
}
</script>

<style>
    .block{
        font-size: 50px;
        width: 400px;
        border-radius:20px;
        background: #ffb3b3;
        color: white;
        text-align: center;
        padding: 100px 0;
        margin: 40px auto;
    }
</style>