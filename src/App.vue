<template>
    <div class="app">
        <TogHeader></TogHeader>
        <TogNewsList></TogNewsList>
    </div>
</template>

<script>
    import { TogHeader, TogNewsList } from 'features';

    export default {
        name: 'app',
        components: {
            TogHeader,
            TogNewsList,
        },
    };

</script>

<style lang="scss">
    @import "./styles/util.scss";
    body, html, .app {
        @include size(100%, 100%);
    }

    @font-face {
        font-family: 'iconfont';  /* project id 244726 */
        src: url('//at.alicdn.com/t/font_ebvgx0lrm7u2qpvi.eot');
        src: url('//at.alicdn.com/t/font_ebvgx0lrm7u2qpvi.eot?#iefix') format('embedded-opentype'),
        url('//at.alicdn.com/t/font_ebvgx0lrm7u2qpvi.woff') format('woff'),
        url('//at.alicdn.com/t/font_ebvgx0lrm7u2qpvi.ttf') format('truetype'),
        url('//at.alicdn.com/t/font_ebvgx0lrm7u2qpvi.svg#iconfont') format('svg');
    }
    .icon {
        font-family: 'iconfont';
        font-style: normal;
    }
</style>
