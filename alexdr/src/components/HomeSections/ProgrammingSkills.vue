<template>
    <div>
        <div v-if="isMobile" className="fade-buffer mobile" />
        <div className="fade-buffer" v-else />
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
    @import '@/styles/ProgrammingSkills/ProgrammingSkills.scss';
</style>
