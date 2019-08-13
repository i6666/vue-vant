<template>
    <van-cell-group title="简单设置">
        <van-cell title="单元格" value="内容" />
        <van-cell  value="内容" />
        <van-cell title="单元格" value="内容" label="描述信息" />
        <van-cell title="地址" icon="location-o" />
        <van-cell title="通用" is-link />
        <van-cell title="展开" arrow-direction="down" is-link />
        <van-cell title="会员中心" is-link to="user" />
    </van-cell-group>

</template>

<script>
    import {Cell,CellGroup} from 'vant'

    export default {
        components: {
            [Cell.name]: Cell,
            [CellGroup.name]: CellGroup
        }
    };
</script>
