<template>
  <div v-if="true" class="loading">
        <div >
            <lottie
                :width="200"
                :height="200"
                :options="lottieOptions"
                @animCreated="handleAnimation"
                class="newText"
            />
        </div>
  </div>
</template>

<script>
import lottie from "vue-lottie/src/lottie.vue";
import * as animationData from "@/assets/animations/covers.json"; //covers
export default {
  components: {
    lottie,
  },
  data() {
    return {
      loading: true,
      anim: null, // for saving the reference to the animation
      lottieOptions: { animationData: animationData.default },
    };
  },
  methods: {
    handleAnimation: function(anim) {
      this.anim = anim;
    },
    start() {
      this.loading = true;
    },
    finish() {
      this.loading = false;
    },
  },
};
</script>

<style>
.loading {
  display: flex;
}
.newText{
  font-family: 'Rubik', arial, sans-serif;
  font-weight: lighter;
  font-size: 28px;
  line-height: 120%;
}
.loadingOld {
  background: white;
  width: 100%;
  height: 100vh;
  display: grid;
  place-items: center;
  position: absolute;
  top: 0;
  left: 0;
}
</style>