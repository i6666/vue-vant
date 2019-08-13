<template>
    <div id="button"><p align="center">按钮类型</p>
        <van-button type="default">默认</van-button>
        <van-button type="primary">主要按钮</van-button>
        <van-button type="warning" icon="star-o" >警示按钮</van-button>
        <van-button type="danger">危险按钮</van-button>
        <van-button type="info">危险按钮</van-button>
        <p align="center">朴素按钮</p>
        <van-button plain type="default">默认</van-button>
        <van-button plain type="primary">主要按钮</van-button>
        <van-button plain type="warning">警示按钮</van-button>
        <van-button plain type="danger">危险按钮</van-button>
        <van-button plain type="info">信息按钮</van-button>
        <p align="center">禁用按钮</p>
        <van-button disabled type="info">禁用</van-button>
        <p align="center">加载中按钮</p>
        <van-button loading type="info"></van-button><br/>
        <van-button loading loading-type="spinner" type="info" ></van-button><br/>
        <van-button loading loading-type="spinner" size='mini' type="info" loading-text="加载中。。" ></van-button><br/>
    </div>
</template>
<script>
    import {Button} from 'vant'

    export default {
        components: {
            [Button.name]: Button,
        }
    };
</script>
