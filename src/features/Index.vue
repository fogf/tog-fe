<template>
    <div class="feature-index">
        <TogDividerBar class="divider-bar"></TogDividerBar>
    </div>
</template>

<script>
    import { TogDividerBar } from 'components';

    export default {
        name: 'TogIndex',
        components: {
            TogDividerBar,
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
