<template>
  <div class="header">
    <div class="content">
      <div class="left-bar">
        <img alt="logo" src="../assets/logo.svg">
      </div>
      <MqResponsive target="xs">
        <div class="mobile-menu"><img alt="user" src="../assets/mobile-menu-icon.svg"></div>
      </MqResponsive>
      <MqResponsive :target="['sm', 'md', 'ld', 'xl', 'xxl']">
        <div class="right-bar">
          <a href="#" class="menu-item">
            Leaderboard
          </a>
          <div class="between"></div>
          <div class="asc"><img alt="asc" src="../assets/asc.svg"></div>
          <div class="user-image"><img alt="user" src="../assets/user.svg"></div>
        </div>
      </MqResponsive>
    </div>
  </div>
</template>

<script>
import {onMounted} from "vue";
import {MqResponsive} from "vue3-mq";
import {updateBreakpoints} from "vue3-mq";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Header',
  components: {MqResponsive},
  props: {
    msg: String
  },

  setup() {
    onMounted(() => {
      updateBreakpoints({
        preset: "tailwind"
      })
    })
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="scss">
@import "../scss/app.scss";
</style>
