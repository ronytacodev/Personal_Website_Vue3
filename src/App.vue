<template>
  <div>
    <the-personal-data />
    <the-about />
    <the-skills />
  </div>
</template>

<script>

import ThePersonalData from '@/components/home/ThePersonalData'
import TheAbout from '@/components/home/TheAbout'
import TheSkills from '@/components/home/TheSkills'

export default {
  name: 'App',
  components: {
    ThePersonalData,
    TheAbout,
    TheSkills
  }
}
</script>

<style>
* {
  margin: 0px;
  padding: 0px;
}
</style>
