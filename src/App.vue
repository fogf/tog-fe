<template>
    <TogHeader></TogHeader>
</template>

<script>
    import { TogHeader } from 'features';

    export default {
        name: 'app',
        components: {
            TogHeader,
        },
    };

</script>

<style lang="scss">
    @import "./styles/util.scss";
    body, html {
        @include size(100%, 100%);
    }
</style>
