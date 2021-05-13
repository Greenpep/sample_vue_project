<template>
    <div class="block">
        click to applause
    </div>
</template>

<script>
export default {
    props: ['applause_counter'],
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