<template>
    <div class="feature-user-panel">
        <Avatar size="52" circle="true"></Avatar>
        <p class="nick">这是用户昵称</p>
        <Dropdown class="dropdown"></Dropdown>
    </div>
</template>

<script>
    import { Avatar, Dropdown } from 'components';

    export default {
        name: 'UserPanel',
        components: {
            Avatar,
            Dropdown,
        },
    };
</script>

<style lang="scss">
    @import "../styles/util.scss";
    .feature-user-panel {
        @include size(180px, 100%);
        display: flex;
        align-items: center;
        justify-content: center;
        color: #333;
        position: relative;

        & > .nick {
            margin-left: 12px;
        }
        & > .dropdown {
            position: absolute;
            top: 70px;
            display: none;
        }
        &:hover {
            background-color: #F7F7F7;
            & > .dropdown {
                display: block;
            }
        }
    }
</style>
