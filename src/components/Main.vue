<template>
  <div class="main-container">

    <MqResponsive class="main" :target="['sm', 'md', 'ld', 'xl', 'xxl']">
      <div class="content-desktop">
        <h1 class="header-content">3 Favorites</h1>

        <div class="favorites-container">
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <span>Online</span>
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <span>Offline</span>
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <span>Online</span>
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
        </div>
      </div>
    </MqResponsive>
    <MqResponsive class="main" target="xs">
      <div class="content-mobile">
        <h1 class="header-content">Favorites 4/4</h1>

        <div class="favorites-container">
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
          <div class="favorite-items">
            <div class="close-container">
              <a href="#" class="close">
                <img alt="close" src="../assets/close.svg">
              </a>
            </div>
            <div class="user-container">
              <img src="../assets/favorite-user.svg">
              <h5>Name surname</h5>
              <span class="handle">@handle</span>
              <button class="message">Message</button>
              <button class="send-tip">Send Tip</button>
            </div>
          </div>
        </div>
      </div>
    </MqResponsive>

  </div>
</template>

<script>
import {onMounted} from "vue";
import {MqResponsive} from "vue3-mq";
import {updateBreakpoints} from "vue3-mq";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Main',
  props: {
    msg: String
  },
  components: {MqResponsive},
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

</style>
