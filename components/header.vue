<template>
  <b-nav>
    <b-nav-item v-for="item in navData" :key="item.link">
      <nuxt-link :to="item.link">
        {{ item.navName }}
      </nuxt-link>
    </b-nav-item>
  </b-nav>
</template>
<script>
export default {
  data () {
    return {
      navData: [
        {
          navName: '首页',
          link: '/'
        },
        {
          navName: 'demo',
          link: '/demo'
        }
      ]
    }
  }
}
</script>

<style scoped lang="less">

</style>
