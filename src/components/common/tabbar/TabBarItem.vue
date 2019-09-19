<template>
    <div class="tab-bar-item" @click="itemClick">

        <div v-if="!isActive">
            <slot name="item-icon"></slot>
        </div>
        <div v-else>
            <slot name="item-icon-active"></slot>
        </div>
        <div :class="{active:isActive}">
            <slot name="item-text"></slot>
        </div>


    </div>
</template>

<script>
    export default {
        name: '',

        computed: {
            isActive() {
                return this.$route.path.indexOf(this.link) !== -1
            }
        },
        props: {
            link: String
        },
        methods: {
            itemClick() {
                this.$router.replace(this.link)
            }
        }
    }
</script>

<style>
    .tab-bar-item {
        flex: 1;
        text-align: center;
        height: 49px;
        background-color: #f6f6f6;
        font-size: 14px;
        margin-top: 3px;
        vertical-align: middle;
        margin-bottom: 2px;

    }

    .tab-bar-item img {
        width: 24px;
        height: 24px;
    }

    .active {
        color: red;
    }
</style>