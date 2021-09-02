<template>
  <div class="home">
    <Introduction /> <!-- Introduction -->
    <div>
      <MobileWarning v-if="!isMobile == false" />  <!-- Mobile Warning -->
    </div>
    <ProgrammingSkills :isMobile="!isMobile == false"/>

  </div>
</template>

<script lang="ts">
import Introduction from '../components/HomeSections/Introduction.vue'
import MobileWarning from '../components/HomeSections/MobileWarning.vue'
import ProgrammingSkills from '../components/HomeSections/ProgrammingSkills.vue'

import { isMobile } from 'mobile-device-detect'

export default {
	name: 'Home',
	components: { Introduction, MobileWarning, ProgrammingSkills },
	setup () {
		return { isMobile }
	}
}
</script>
