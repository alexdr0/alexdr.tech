<template>
    <div>
        <div className="introdiv">
            <div className="introdiv-text">
                <h class="header">
                    &nbsp;  <Typewriter :speed="200" :nextWordInterval="3000" :deleteSpeed="150"  :words="['alexdr', 'alexdr0', ' xander', 'alex']" ></Typewriter>
                </h>
            </div>
            <span class="subtext">Programmer, Student, Enteprenur and a little bit of everything else</span><br>
            <div class="fade-in-down">
                <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-caret-down-fill down-animation" viewBox="0 0 16 16">
                    <path d="M7.247 11.14 2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z"/>
                </svg>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import Typewriter from '../Typewriter.vue'
export default {
	name: 'Introduction',
	components: { Typewriter },
	setup () {
		function isMobile () {
			if (/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
				return true
			} else {
				return false
			}
		}
		return { isMobile }
	}
}
</script>

<style lang="scss" scoped>
    @import '@/styles/introdiv.scss';
</style>
