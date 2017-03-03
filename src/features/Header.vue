<template>
    <header class="feature-header">
        <div class="nav-search-container">
            <TogNav>
                <TogNavItem name="首页" selected="true"></TogNavItem>
                <TogNavItem name="电影"></TogNavItem>
                <TogNavItem name="游戏"></TogNavItem>
                <TogNavItem name="书籍"></TogNavItem>
            </TogNav>
            <TogSearch></TogSearch>
        </div>
        <TogUserPanel></TogUserPanel>
    </header>
</template>

<script>
    import { TogNav, TogNavItem, TogSearch } from 'components';
    import TogUserPanel from './UserPanel';

    export default {
        name: 'TogHeader',
        components: {
            TogNav,
            TogNavItem,
            TogSearch,
            TogUserPanel,
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
