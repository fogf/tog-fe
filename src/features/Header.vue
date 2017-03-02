<template>
    <header class="feature-header">
        <Nav>
            <NavItem name="首页" selected="true"></NavItem>
            <NavItem name="电影"></NavItem>
            <NavItem name="游戏"></NavItem>
            <NavItem name="书籍"></NavItem>
        </Nav>
        <Search></Search>
    </header>
</template>

<script>
    import { Nav, NavItem, Search } from 'components';

    export default {
        name: 'Header',
        components: {
            Nav,
            NavItem,
            Search,
        },
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .feature-header {
        @include size(100%, 70px);
        background-color: white;
        box-shadow: 0px 1px 4px #ccc;
        padding: 0px 30px;
        display: flex;
    }
</style>
