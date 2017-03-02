<template>
    <header class="feature-header">
        <div class="nav-search-container">
            <Nav>
                <NavItem name="首页" selected="true"></NavItem>
                <NavItem name="电影"></NavItem>
                <NavItem name="游戏"></NavItem>
                <NavItem name="书籍"></NavItem>
            </Nav>
            <Search></Search>
        </div>
        <UserPanel></UserPanel>
    </header>
</template>

<script>
    import { Nav, NavItem, Search } from 'components';
    import UserPanel from './UserPanel';

    export default {
        name: 'Header',
        components: {
            Nav,
            NavItem,
            Search,
            UserPanel,
        },
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .feature-header {
        @include size(100%, 70px);
        background-color: white;
        box-shadow: 0px 1px 5px #ccc;
        padding: 0px 30px;
        display: flex;
        justify-content: space-between;
        box-sizing: border-box;

        & > .nav-search-container {
            display: flex;
        }
    }
</style>
