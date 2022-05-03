<template>
    <div class="card">
        <div class="info">
            <photo/>
            <div class="letters">
                <h1 class="name">Ada Lovelace</h1>
                <h1 class="city">São Paulo - SP</h1>
                <h2 class="job">Software Engineer</h2>
            </div>
        </div>
        <div class="about">
            <contact/>
        </div>
        <trigger class="trigger"/>
    </div>
</template>

<script>
import Contact from './Contact.vue';
import Photo from './Photo.vue';
import Trigger from './Trigger.vue';

export default {
    components: { Photo, Contact, Trigger, },
    name: 'Card'
};
</script>

<style lang="scss" scoped>
.card {
    height: 700px;
    width: 500px;
    background-color: $purple;
    border: 3px solid $gold;
    border-radius: 50px 5px 0 0;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;

    .info {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        height: 40%;
        padding: 10px;

        .letters {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
        }
            .name{
                font-family: 'Rubik Mono One', sans-serif;
                color: $white;
                font-weight: 800;
                width: 100%;
                text-align: center;
            }
            .city {
                width: 100%;
                color: $gold;
                font-size: 12px;
                text-align: center;
                margin-bottom: 0;
                margin-top: 0;
            }
            .job {
                font-size: 30px;
                font-weight: bold;
                width: 100%;
                text-align: center;
            }
        }
    .about{
        height: 20%;
        margin-right: 200px;
        padding-top: 150px;
    }
    .trigger{
        margin-top: 75px;
    }
}
</style>