<script>
export default {
    props : ['img', 'title']
}
</script>
<template>
    <li>
        <img :src="img" :alt="title">
        <h6>{{ title }}</h6>
    </li>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
li {
    padding: 13px;
    padding-bottom: 0;
    margin-bottom: 13px;
    cursor: pointer;
    img {
        display: block;
        width: 100%;
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: center top;
    }
    h6 {
        font-size: $f-size-series;
        text-transform: uppercase;
        font-weight: bold;
        padding: 20px 0;
    }
    &:hover{
        border: 1px solid $br-primary;
        img {
            filter: grayscale(1);
        }

    }
}
</style>