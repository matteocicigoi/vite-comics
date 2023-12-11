<script>
export default {};
</script>
<template>
    <div>
        <span>Current Series</span>
    </div>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
    div {
        width: $size;
        transform: translate(-50%, -50%);
        position: absolute;
        top: 400px;
        left: 50%;

        span {
            text-transform: uppercase;
            font-weight: bold;
            color: $text-tertiary;
            background-color: $bg-current;
            padding: 15px 30px;
            font-size: $f-size-current;
        }
    }
</style>