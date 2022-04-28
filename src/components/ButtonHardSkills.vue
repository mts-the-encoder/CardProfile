<template>
    <input class="hs" type="button" value="Hard Skills">
</template>

<script>
export default {
    name: 'HardSkills'
}
</script>

<style lang="scss" scoped>
.hs {
    height: 50px;
    width: 200px;
    color: $white;
    background-color: $black;
    border: 1px solid $gold;
    border-radius: 4px;
    font-weight: bold;
    font-size: 18px;
    cursor: pointer;
    margin-left: 100px;
    margin-top: 100px;
}
// vou testar isso dps, pra ver se fica legal
.hs:hover {
    background-color: $white;
    color: $black;
}
</style>