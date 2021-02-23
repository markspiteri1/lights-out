<template>
  <div class="gridcell" :class="getClass()"></div>
</template>

<script>
export default {
  name: "lightsOutCell",
  props: {
    isOn: {
      type: Boolean,
    },
  },
  methods: {
    getClass() {
      if (!this.isOn) {
        return "on";
      }
      return "off";
    },
  },
};
</script>

<style lang="scss">
.gridcell {
  height: 35px;
  width: 35px;
  border-radius: 6px;
  cursor: pointer;
}
.off {
  background: radial-gradient(
    circle,
    rgba(142, 250, 142, 1) 29%,
    rgba(31, 98, 31, 1) 100%
  );
}
.on {
  background-color: red;
}
</style>
