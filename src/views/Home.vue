<template lang="pug">
  .home
    //- img(alt="Vue logo" src="../assets/logo.png")
    Contact(msg="Welcome to Your Vue.js App")
    Menu
    NTHU
    TopSlash
    Activity
    ButtomSlash
    Net
    Icon
</template>

<script>
// @ is an alias to /src
import Contact from '@/components/Contact.vue'
import NTHU from '@/components/NTHU.vue'
import Menu from '@/components/Menu.vue'
import TopSlash from '@/components/TopSlash.vue'
import Activity from '@/components/Activity.vue'
import ButtomSlash from '@/components/ButtomSlash.vue'
import Net from '@/components/Net.vue'
import Icon from '@/components/Icon.vue'

export default {
  // name: 'Home',
  components: {
    Contact,
    NTHU,
    Menu,
    TopSlash,
    Activity,
    ButtomSlash,
    Net,
    Icon
  }
}
</script>
<style lang="sass">
.home
  min-height: 2200px
</style>
