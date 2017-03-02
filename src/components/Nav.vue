<template>
    <nav class="component-nav">
        <ul>
            <slot>
                no nav item
            </slot>
        </ul>
    </nav>
</template>

<script>
    export default {
        name: 'Nav',
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .component-nav {
        @include size(auto, 100%);
        display: inline-block;

        & > ul {
            display: flex;
            margin: 0;
            padding: 0;
            @include size(auto, 100%);
        }
    }
</style>
