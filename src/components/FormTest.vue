<template>
  <div>
    <ul id="errorDataList" v-if="errors">
      <li id="errorDataListItem" v-for="error in errors" :key="error.data">{{ error.data }}</li>
    </ul>

    <form action="#" method="get"
      @submit="form_submit"
    >
      <input type="submit" />
    </form>

  </div>
</template>

<script>
export default {
  name: 'formTest',
  data () {
    return {
      errors: [
        { data: 'err01' }
      ]
    }
  },
  methods: {
    form_submit: function () {
      const errData = {
        data: 'err:' + errCount
      }
      this.errors.push(errData)
    }
  }
}

let errCount = 0

</script>

<style scoped>

ul#errorDataList {
  all: initial;
  text-align: center;
  list-style: none;
}

li#errorDataListItem {
  all: initial;
}

</style>
