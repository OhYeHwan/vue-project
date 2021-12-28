<template>
  <form v-bind:class="size">
    <input type="text" placeholder="소환사명, 소환사명, ..." />
    <!-- class 바인딩 다른 방식 적용해보기 -->
    <button
      :class="{
        button_normal: size === 'normal',
        button_small: size === 'small',
      }"
      @click="searchUser"
    >
      .GG
    </button>
  </form>
</template>

<script>
export default {
  props: {
    size: {
      type: String,
      required: false,
      default: "normal",
    },
  },
  data() {
    return {
      user_name: "",
    };
  },
  methods: {
    searchUser(e) {
      e.preventDefault();
      console.log("1");
      // 로직
      this.user_name = "";
    },
  },
};
</script>

<style>
form {
  display: flex;
  align-items: center;
  background-color: #fff;
}

.normal {
  height: 50px;
}

.small {
  width: 350px;
  height: 30px;
}

input {
  width: 624px;
  padding-left: 10px;
  margin: 0;
  border: none;
  outline: none;
  color: rgb(140, 140, 140);
}

button {
  margin: 0 10px 0 10px;
  border: none;
  color: #fff;
  background-color: rgb(75, 166, 248);
}

.button__normal {
  width: 50px;
  height: 30px;
}

.button__small {
  width: 40px;
  height: 20px;
  font-size: 10px;
}
</style>
