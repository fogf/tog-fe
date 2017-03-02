<template>
    <img
        src="https://ooo.0o0.ooo/2017/01/21/58831ded8aa6d.jpg?imageView2/2/w/40/h/40"
        class="component-avatar" :class="{ circle }"
        :style="{ width: `${size}px`, height: `${size}px` }"
    />
</template>

<script>
    export default {
        name: 'Avatar',
        props: ['size', 'circle'],
    };
</script>

<style lang="scss">
    .component-avatar {
        &.circle {
            border-radius: 50%;
        }
    }
</style>
