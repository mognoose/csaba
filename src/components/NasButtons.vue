<template>
  <div class="block">
    <button v-for="button in buttons" :key="button.url">
      <a :href="button.url" target="_blank">
        <div class="box">
          <img class="icon" alt="" :src="button.icon" />
          {{ button.label }}
        </div>
      </a>
    </button>
  </div>
</template>

<script>
export default {
  props: {
    buttons: {
      type: Array,
      required: true,
    },
  },
  mounted() {
    window.addEventListener(
      "keyup",
      function (e) {
        window.open(this.buttons[e.key - 1].url, "_blank", "noreferrer");
      }.bind(this)
    );
  },
};
</script>

<style lang="scss" scoped>
.content {
  text-align: center;
  margin: 0 auto;
  padding: 0;
}
.box {
  background-color: rgba(255, 255, 255, 0.3);
  display: inline-block;
  width: 70px;
  height: 70px;
  padding: 20px;
  text-align: center;
  border: 1px solid black;
  border-radius: 5px;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.8);
}
.icon {
  width: 50px;
  height: 50px;
  margin-bottom: 5px;
}

a:link,
a:visited {
  margin: 10px;
  color: #000;
  text-decoration: none;
  display: inline-block;
}

a:hover,
a:active {
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.8);
}

button {
  background: none;
  border: none;
}
</style>
