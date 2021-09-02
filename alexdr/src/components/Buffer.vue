<template>
	<div>
		<div style="width:100%;" id="buffer"> </div>
	</div>
</template>

<script lang='ts'>
import { ref, onMounted } from 'vue'
export default {
	name: 'Buffer',
	props: {
		buffer: {
			type: String,
			required: true
		}
	},
	setup (props:any) {
		onMounted(() => {
			document.getElementById('buffer')!.style.height = props.buffer + 'pt'
		})
	}
}
</script>
