<template>
    <div class="categoria">
        <img class="beneficio_icon" :src="img">
        <br>
        <span> {{ span }} </span>
    </div>
</template>

<script>
export default{
    props:['img', 'span']
}
</script>

<style scoped>
    .categoria {
        cursor: pointer;
        font-size: 12px;
        text-align: center;
    }
</style>