<script>

export default {
    name: "AppJumbotron",

}

</script>

<template>
    <div id="jumbotron"></div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

#jumbotron {
    height: 350px;
    background-image: url(../assets/images/jumbotron.jpg);
    background-size: cover;
}
</style>