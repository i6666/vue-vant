<template>
    <van-address-edit
            :area-list="areaList"
            show-postal
            show-delete
            show-set-default
            show-search-result
            :search-result="searchResult"
            @save="onSave"
            @delete="onDelete"
            @change-detail="onChangeDetail"
    />
</template>
<script>
    import {AddressEdit, Toast, Area} from 'vant';

    export default {
        components: {
            [AddressEdit.name]: AddressEdit,
            [Area.name]: Area
        },
        data() {
            return {
                areaList: {
                    province_list: {
                        550000: '北京市',
                        120000: '天津市'
                    },
                    city_list: {
                        550100: '北京市',
                        550200: '县',
                        120100: '天津市',
                        120200: '县'
                    },
                    county_list: {
                        550101: '东城区',
                        550102: '西城区',
                        550105: '朝阳区',
                        550106: '丰台区',
                        120101: '和平区',
                        120102: '河东区',
                        120103: '河西区',
                        120104: '南开区',
                        120105: '河北区',
                    }
                },
                searchResult: []
            }
        },

        methods: {
            onSave() {
                Toast('save');
            },
            onDelete() {
                Toast('delete');
            },
            onChangeDetail(val) {
                if (val) {
                    this.searchResult = [{
                        name: '黄龙万科中心',
                        address: '杭州市西湖区'
                    }];
                } else {
                    this.searchResult = [];
                }
            }
        }
    };
</script>
