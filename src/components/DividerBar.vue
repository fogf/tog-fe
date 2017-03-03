<template>
    <div class="component-divider-bar">
        <i class="icon">&#xe628;</i>
        <span>最新动态</span>
    </div>
</template>

<script>
    export default {
        name: 'TogDividerBar',
    };
</script>

<style lang="scss">
    .component-divider-bar {
        border-bottom: #ccc 1px solid;
        padding-bottom: 8px;
        display: flex;
        align-items: center;

        $textColor: #666;
        & > i {
            color: $textColor;
            font-size: 24px;
        }
        & > span {
            color: $textColor;
            margin-left: 5px;
        }
    }
</style>
