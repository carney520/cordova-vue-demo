<template lang="jade">
 h1 DEMO
 div.test {{ num }}
 button(@click="increase") INCREASE
 a(v-link="{name: 'foo'}") foo
</template>

<script>
import { increase } from 'actions/test'

export default {
  vuex: {
    getters: {
      num: (state) => state.test.num
    },

    actions: {
      increase
    }
  }
}
</script>

<style lang="scss">
</style>