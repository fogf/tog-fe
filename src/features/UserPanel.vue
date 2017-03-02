<template>
    <div class="feature-user-panel">
        <Avatar size="52" circle="true"></Avatar>
        <p>这是用户昵称</p>
    </div>
</template>

<script>
    import { Avatar } from 'components';

    export default {
        name: 'UserPanel',
        components: {
            Avatar,
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

        & > p {
            margin-left: 12px;
        }
    }
</style>
