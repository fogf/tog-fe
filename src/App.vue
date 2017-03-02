<template>
    <Header></Header>
</template>

<script>
    import { Header } from 'features';

    export default {
        name: 'app',
        components: {
            Header,
        },
    };

</script>

<style lang="scss">
    @import "./styles/util.scss";
    body, html {
        @include size(100%, 100%);
    }
</style>
