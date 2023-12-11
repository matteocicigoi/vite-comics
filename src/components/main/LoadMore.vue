<script>
export default {};
</script>
<template>
    <button>
        load more
    </button>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
    button {
        text-transform: uppercase;
        background-color: $bg-current;
        color: $text-tertiary;
        font-weight: bold;
        padding: 12px 60px;
        display: block;
        margin: 0 auto;
        border: none;
        cursor: pointer;
    }
</style>