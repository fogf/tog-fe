<template>
    <div class="component-dropdown">
        <ul>
            <li>我的主页</li>
            <li>设置</li>
            <li>退出登录</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'Dropdown',
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .component-dropdown {
        & > ul {
            padding: 10px 0px;
            margin: 0;
            background-color: #F6F6F6;

            & > li {
                list-style: none;
                @include size(180px, 40px);
                line-height: 40px;
                padding: 0px 50px;
                box-sizing: border-box;
                cursor: pointer;
                user-select: none;
                @include animate(hover, background-color, rgba(#979797, 0.12), 0.5s);
            }
        }
    }
</style>
