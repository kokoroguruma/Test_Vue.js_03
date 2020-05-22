<template>

<div>
  <h3>プロフィール</h3>
  <h4> {{ profileData }} </h4>
  <p> {{ msg2 }} </p>
</div>

</template>

<script>
export default {
  name: 'Profile',
  data () {
    return {
      profileData: 'p-Data',
      msg2: 'aaa'
    }
  }
}
</script>

<style scoped>

</style>
