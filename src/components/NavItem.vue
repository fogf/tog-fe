<template>
    <li class="component-nav-item">
        <p :class="{ selected: selected }">
            {{ name }}
        </p>
    </li>
</template>

<script>
    export default {
        name: 'NavItem',
        props: ['name', 'selected'],
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .component-nav-item {
        @include size(80px, 100%);
        list-style: none;
        padding: {
            left: 10px;
            right: 10px;
        }
        cursor: pointer;
        box-sizing: border-box;
        @include animate(hover, background-color, #f1f1f1, 0.5s);

        & > p {
            @include size(100%, 100%);
            margin: 0;
            text-align: center;
            padding-top: 6px;
            line-height: 70px - 6px * 2;
            font-size: 18px;
            box-sizing: border-box;
            &.selected {
                border-bottom: #FF7171 6px solid;
            }
        }
    }
</style>
