<template>
    <div class="feature-index">
        <TogDividerBar class="divider-bar"></TogDividerBar>
        <TogNews></TogNews>
        <TogNews></TogNews>
    </div>
</template>

<script>
    import { TogDividerBar } from 'components';
    import TogNews from './News';

    export default {
        name: 'TogNewsList',
        components: {
            TogDividerBar,
            TogNews,
        },
    };
</script>

<style lang="scss">
    .feature-index {
        padding: 0px 30px;

        & > .divider-bar {
            margin-top: 48px;
        }
    }
</style>
