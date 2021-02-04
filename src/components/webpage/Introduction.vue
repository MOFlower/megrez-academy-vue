<template>
  <div class="background">
    <div class="title">
      ABOUT us
      <div class="text">
        Mission： Michigan Youth Empowerment Foundation (mYe) is a 501(c3)
        nonprofit foundation established to promote STEAM (Science, Technology,
        Engineering, Arts, and Math) programs to students K-12 and empower them
        to thrive in the new technological world.
      </div>
      <div class="image">
        <img src="../../assets/img/logo.png" alt />
      </div>
    </div>
    <div class="login-btn">
      <el-button type="primary" @click="Jump">LOG IN / SIGN UP</el-button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    Jump() {
      this.$router.push("login");
    },
  },
};
</script>

<style scoped>
.title {
  position: absolute;
  left: 15%;
  top: 5%;
  font-family: serif;
  font-weight: 700;
  font-size: 100px;
  color: saddlebrown;
}
.text {
  position: relative;
  top: 100px;
  left: 60%;
  width: 40%;
  font-size: 35px;
  color: chocolate;
}
.image {
    position: relative;
    top: -550px;
    left: -200px;
}
.background {
  position: relative;
  width: 100%;
  height: 100%;
  background-image: url(../../assets/img/slider.jpg);
  background-size: 100%;
}
.login-btn button {
  position: absolute;
  top: 5%;
  right: 5%;
  width: 10%;
  height: 50px;
  margin-bottom: 200px;
}
</style>