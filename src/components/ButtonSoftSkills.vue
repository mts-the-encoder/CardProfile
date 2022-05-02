<template>
    <label for="SoftSkills" class="ss" >
        <input class="check" type="checkbox" id="SoftSkills">
        <span>Soft Skills</span>
    </label>
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
    display: flex;
    align-items: center;
    justify-content: center;

    .check {
        visibility: hidden;
        width: 100%;
        height: 100%;
    }
}
</style>