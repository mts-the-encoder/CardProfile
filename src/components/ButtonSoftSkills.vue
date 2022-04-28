<template>
    <input class="ss" type="button" value="Soft Skills">
</template>

<script>
export default {
    name: 'SoftSkills'
}
</script>

<style lang="scss" scoped>
.ss {
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
.ss:hover {
    background-color: $white;
    color: $black;
}
</style>