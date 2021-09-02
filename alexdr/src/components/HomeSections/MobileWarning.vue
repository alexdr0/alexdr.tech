<template>
    <div style="margin:0;">
        <div class="top" />
        <div class="mainContentArea">
            <Buffer buffer="20" />
            <h1> Please use a desktop browser for the best user experience. </h1>
        </div>
    </div>
</template>

<script lang="ts">
import Buffer from '../Buffer.vue'
export default {
	name: 'MobileWarning',
	components: { Buffer }
}
</script>

<style lang="scss" scoped>

    .top{
        height:25pt;
        width:100%;
        background-image: linear-gradient(180deg, #0338be, darkslategray);
        margin:none;
    }

    .mainContentArea{
        height:100vh;
        width:100%;
        background:darkslategray;
        padding:10%;
    }

    h1{
        font-size:30pt;
        color:white;
        font-family:Roboto Mono;
        font-weight:bold;
    }

</style>
