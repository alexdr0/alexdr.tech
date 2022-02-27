<template>
  <div class="home">
    <Introduction /> <!-- Introduction -->
    <div>
      <MobileWarning v-if="!isMobile == false" />  <!-- Mobile Warning -->
    </div>
    <Profile :isMobile="!isMobile == false"/>

  </div>
</template>

<script lang="ts">
import Introduction from '../components/HomeSections/Introduction.vue'
import MobileWarning from '../components/HomeSections/MobileWarning.vue'
import Profile from '../components/HomeSections/Profile.vue'

import { isMobile } from 'mobile-device-detect'

export default {
	name: 'Home',
	components: { Introduction, MobileWarning, Profile },
	setup () {
		return { isMobile }
	}
}
</script>
