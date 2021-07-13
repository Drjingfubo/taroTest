<template>
  <view class="index">
    <view>
      <img src="" alt="" />
    </view>
    <input type="text" :focus="isFocus" />
    <div @click="focu()">123</div>
  </view>
</template>

<script lang="ts">
import { ref } from "vue";
export default {
  name: "Index",
  components: {},
  setup() {
    const isFocus = ref(false);
    const focu = () => {
      isFocus.value = true;
    };

    return {
      isFocus,
      focu,
    };
  },
};
</script>

<style lang="css">
.index {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
.btn .nut-button {
  width: 150px;
  height: 50px;
  margin-top: 30px;
  font-size: 20px;
}
.nut-toast-text {
  font-size: 20px;
}
input {
  width: 100px !important;
  height: 30px;
  border: 1px solid red !important;
}
</style>
