<template>
    <div class="profile">
        <div class="circle">

        </div>
    </div>
</template>

<script>
export default {
    name: 'Photo'
}
</script>

<style lang="scss" scoped>
.profile {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    background-color: $white;
    filter: drop-shadow(10px 10px 10px $black);
    margin-left: 500px;

    .circle {
    width: 200px;
    height: 200px;
    background-image: url("../assets/imgs/ada.png");
    background-size: 150px;
    background-repeat: no-repeat;
    border-radius: 50%;
    border: 2px solid $black;
    background-position-x: 20px;
    background-position-y: 0px;
    }
}

</style>