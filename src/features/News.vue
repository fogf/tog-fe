<template>
    <div class="feature-news">
        <TogAvatar size="35"></TogAvatar>
        <div class="content">
            <p class="nick-time">许卡拉 发表了影评 • 7 小时前</p>
            <p class="text">看了首映，满满的失望，想看的片段都被删了。。</p>
            <div class="share-item">
                <img src="http://cdn.suisuijiang.com/message_1488532358771.jpeg" />
                <div class="name">
                    <p>生化危机：终章 Resident Evil: The Final Chapter (2016)</p>
                </div>
                <div class="score">
                    <span>7</span>
                    <span>.4</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import { TogAvatar } from 'components';

    export default {
        name: 'TogNews',
        components: {
            TogAvatar,
        },
    };
</script>

<style lang="scss">
    @import "../styles//util.scss";
    .feature-news {
        display: flex;
        margin-top: 20px;

        & > .content {
            margin-left: 15px;
            & > .nick-time {
                color: #999;
                font-size: 14px;
                margin: 8px 0px;
            }
            & > .text {
                color: #666;
                font-size: 14px;
                margin: 8px 0px;
            }
            & > .share-item {
                @include size(520px, 112px);
                display: flex;
                overflow: hidden;
                border: #ddd 1px solid;
                border-radius: 5px;

                & > img {
                    @include size(124px, 174px);
                    min-width: 124px;
                }
                & > .name {
                    flex: 1;
                    padding: 8px;
                    & > p {
                        margin: 0;
                    }
                }
                & > .score {
                    @include size(78px, 78px);
                    min-width: 78px;
                    background-color: #FF7171;
                    text-align: center;
                    padding-top: 10px;
                    box-sizing: border-box;
                    align-self: center;
                    margin-right: 17px;
                    & > span {
                        color: white;
                        font-size: 44px;
                        &:nth-child(2) {
                            font-size: 36px;
                        }
                    }
                }
            }
        }
    }
</style>
