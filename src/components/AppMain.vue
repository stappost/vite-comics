<script>
import AppBlueMain from './AppBlueMain.vue'
export default {
    name: "AppMain",
    components: {
        AppBlueMain
    }
}
</script>
<template lang="">
    <main>
        <div class="bg_black">
            <div class="container">
                <h3 class="text-white">
                 --> Content goes here <--
                </h3>
            </div>
        </div>
        <AppBlueMain />
    </main>
</template>
<style lang="scss" scoped>
main {
    margin-top: 20px;

    .bg_black {
        background-color: #000;
        padding: 50px;

        .text-white {
            color: #fff;
        }
    }
}
</style>