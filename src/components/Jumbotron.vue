<script>
export default {
    name: "Jumbotron"
}
</script>
<template lang="">
    <div class="jumbo">
        <div class="container">
            <div class="current">
                CURRENT SERIES
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variabiles' as *;

.jumbo {
    background-image: url("../assets/img/jumbotron.jpg");
    height: 400px;
    margin-top: 20px;
    background-size: cover;
    position: relative;

    .current {
        color: white;
        background-color: $primary;
        position: absolute;
        padding: 10px 20px;
        font-weight: 700;
        bottom: -20px;
    }
}
</style>