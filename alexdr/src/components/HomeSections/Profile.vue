<template>
    <div>
        <div v-if="isMobile" className="fade-buffer mobile" />
        <div className="fade-buffer" v-else />
		<div class="mainarea">
			<div class="halves">
				<img src="@/assets/profilephoto.jpg" class="profilephoto" /><br>
				<span class="profile-name">Alexander Bobo</span>
			</div>
			<div class="halves">
				<div class="skill"></div>
				<div class="skill"></div>
				<div class="skill"></div>
				<div class="skill"></div>
			</div>
		</div>
    </div>
</template>

<script lang="ts">
export default {
	name: 'ProgrammingSkills',
	props: {
		isMobile: {
			type: Boolean,
			required: true
		}
	}
}
</script>

<style lang="scss" scoped>
    @import '@/styles/Profile/Profile.scss';
</style>
