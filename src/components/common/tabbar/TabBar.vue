<template>
    <div id="tab-bar">
        <TabBarItem link="/home">

            <img slot="item-icon" src="@/assets/img/tabbar/home.svg" alt="">
            <img slot="item-icon-active" src="@/assets/img/tabbar/home_active.svg" alt="">
            <div slot="item-text">首页</div>


        </TabBarItem>

        <TabBarItem link="/category">
            <img slot="item-icon" src="@/assets/img/tabbar/category.svg" alt="">
            <img slot="item-icon-active" src="@/assets/img/tabbar/category_active.svg" alt="">
            <div slot="item-text">分类</div>
        </TabBarItem>
        <TabBarItem link="/cart">
            <img slot="item-icon" src="@/assets/img/tabbar/shopcart.svg" alt="">
            <img slot="item-icon-active" src="@/assets/img/tabbar/shopcart_active.svg" alt="">
            <div slot="item-text">购物车</div>
        </TabBarItem>
        <TabBarItem link="/profile">
            <img slot="item-icon" src="@/assets/img/tabbar/profile.svg" alt="">
            <img slot="item-icon-active" src="@/assets/img/tabbar/profile_active.svg" alt="">
            <div slot="item-text">我的</div>
        </TabBarItem>


    </div>

</template>

<script>
    import TabBarItem from '@/components/common/tabbar/TabBarItem.vue'

    export default {
        name: '',
        data() {
            return {}
        },
        components: {TabBarItem}
    }
</script>

<style>
    #tab-bar {
        display: flex;
        position: fixed;
        left: 0;
        right: 0;
        bottom: 0;

        box-shadow: 0 -3px 1px rgba(100 100 100 .08);
    }

</style>
