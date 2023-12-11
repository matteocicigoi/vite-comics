<script>
export default {};
</script>

<template>
    <button>sign-up now!</button>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
    button{
        all: unset;
        border: 2px solid $br-primary;
        text-transform: uppercase;
        color: white;
        cursor: pointer;
        padding: 15px;
        &:hover{
            color: $text-primary;
            background-color: $bg-button;
        }
    }
</style>