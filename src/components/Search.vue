<template>
    <div class="component-search">
        <input placeholder="搜索电影、游戏…">
    </div>
</template>

<script>
    export default {
        name: 'Search',
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .component-search {
        display: flex;
        align-items: center;
        margin-left: 60px;

        & > input {
            @include size(350px, 36px);
            padding-left: 12px;
            border-radius: 2px;
            border: #ccc 1px solid;
            outline: none;
            font-size: 14px;

            $focusColor: #03a9f4;
            @include animate(focus, border-color, $focusColor, 0.2s);
            @include animate(focus, box-shadow, 0px 0px 4px $focusColor, 0.2s);
        }
    }
</style>
