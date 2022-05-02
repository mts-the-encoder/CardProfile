<template>
    <div class="contacts">
        <div class="contact">
            <img class="icon--contact" src="../assets/imgs/github.svg" alt="GitHub">
        </div>
        <div class="contact">
            <img class="icon--contacts" src="../assets/imgs/gmail.svg" alt="Gmail">
        </div>
        <div class="contact">
            <img class="icon--contacts" src="../assets/imgs/linkedin.svg" alt="LinkedIn">
        </div>
        <div class="contact">
            <img class="icon--contacts" src="../assets/imgs/twitter.svg" alt="Twitter">
        </div>
        <div class="contact">
            <img class="icon--contactss" src="../assets/imgs/face.svg" alt="Facebook">
        </div>
        <div class="contact">
            <img class="icon--contacts" src="../assets/imgs/insta.svg" alt="Instagram">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Contact'
}
</script>

<style lang="scss" scoped>
.contacts {
    margin-left: 200px;
    width: 400px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;

    .contact {
        height: 45px;
        width: 45px;
        border-radius: 50%;
        border: 2px solid $black;
        display: flex;
        justify-content: center;
        align-items: center;
        filter: drop-shadow(0px 4px 4px rgba(100, 100, 100, 0.25));
        box-shadow: 1px 1px 0 0 $black;
        cursor: pointer;

        .icon--contact {
            height: 35px;
            filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
        }

        .icon--contacts {
            height: 55px;
            margin-top: 25px;
        }
        .icon--contactss {
            height: 55px;
            margin-top: 22px;
            margin-left: 1.3px;
        }
    }
    .contact:hover{
        background-color: $white;
    
        .icon--contacts:hover {
            filter: drop-shadow(0px 4px 4px $black);
        }

        .icon--contacts:hover {
            filter: drop-shadow(0px 1px 1px $black);
        }
    }
}
</style>