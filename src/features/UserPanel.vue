<template>
    <div class="feature-user-panel">
        <TogAvatar size="52" circle="true"></TogAvatar>
        <p class="nick">这是用户昵称</p>
        <TogDropdown class="dropdown"></TogDropdown>
    </div>
</template>

<script>
    import { TogAvatar, TogDropdown } from 'components';

    export default {
        name: 'TogUserPanel',
        components: {
            TogAvatar,
            TogDropdown,
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
