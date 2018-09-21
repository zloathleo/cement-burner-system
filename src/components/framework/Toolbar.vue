<template>
    <!-- Hero head: will stick at the top -->
    <div class="hero-head" style="border-bottom: 5px solid #e50112;">
        <nav class="navbar ">
            <div class="navbar-brand" v-if="showDrawerIcon">
                <a class="navbar-item" @click="showDrawer">
                    <b-icon icon="view-headline"></b-icon>
                </a>
            </div>
            <div class="navbar-menu">
                <div class="navbar-end">
                    <a class="navbar-item">
                        <b-icon icon="view-headline"></b-icon>
                    </a>
                </div>
            </div>
        </nav>
    </div>
</template>
 
<script>  
export default {
    data() {
        return {
            showDrawerIcon: !this.$globalvar.configMode,//是否loading状态
        }
    },
    methods: {
        showDrawer() {
            this.$globalEventHub.$emit("showDrawer");
        }
    }
}
</script>