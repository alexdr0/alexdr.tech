<template>
  <div class="about">
    <Buffer buffer="50" />
      <div class="contact-me">
        <span class="hdr">Shoot me a msg</span><br>
        <span class="opt">Email me: buisness@alexdr.tech</span><br>
        <span class="opt">Discord: alexdr#0007</span>
      </div>
  </div>
</template>

<style scoped>

.contact-me{
  height: 300pt;
  width: 500pt;

  margin-right: calc(50% - 250pt);
  margin-left: calc(50% - 250pt);
  border-radius: 12pt;
}
.hdr{
  font-size:30pt;
  font-family:inter;
  margin-top: 10pt;
  margin-bottom:20pt;
  font-weight:bold;
}

.opt{
  font-size: 14pt;
  font-family:inter;
}
</style>

<script lang="ts">
import Buffer from '../components/Buffer.vue'

export default {
	name: 'Projects',
	components: { Buffer }
}
</script>
