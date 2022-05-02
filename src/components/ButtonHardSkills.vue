<template>
    <label for="HardSkills" class="hs">
        <input class="check" type="checkbox" id="HardSkills">
        <span>Hard Skills</span>
    </label>
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
    display: flex;
    justify-content: center;
    align-items: center;

    .check {
        display: none;
    }
}
</style>