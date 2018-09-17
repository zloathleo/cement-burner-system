<template>

    <div>
        <section class="hero color-primary-3">
            <Toolbar />
        </section>
        <b-loading :is-full-page="true" :active.sync="isAppLoading"></b-loading>
        <Drawer />

        <main class="main-container">
            <div class="content">
                <router-view></router-view>
            </div>
            <Footer />
        </main>

    </div>

</template>

<style scoped lang="less">
.main-container {
  min-height: 1048px;
  background-color: #f5f5f5;
  .content {
    background-color: white;
    margin: 0px 20px;
    padding: 20px;
    max-width: 100%;
  }
}
</style>


<script> 
import Toolbar from './Toolbar.vue';
import Drawer from './Drawer.vue';
import Footer from './Footer.vue';
export default {
    components: { Toolbar, Drawer },

    data() {
        return {
            isAppLoading: false,//是否loading状态
        }
    },
    beforeMount() {
        let _this = this;
        this.$globalEventHub.$on("appLoading", function (value) {
            _this.isAppLoading = value;
        });
    },
    methods: {
    }
}
</script>