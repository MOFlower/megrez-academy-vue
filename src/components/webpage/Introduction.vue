<template>
  <div class="background">
    <el-container>
      <el-header>
        <el-row :gutter="20">
          <el-col :span="3">
            <img src="../../assets/img/logo.png" />
          </el-col>
          <el-col :span="12">
            <img src="" alt="" />
          </el-col>
          <el-col :span="3">
            <el-link @click="home">HOME</el-link>
          </el-col>
          <el-col :span="3">
            <el-link href="https://myefound.org/">MYE</el-link>
          </el-col>
          <el-col :span="3">
            <el-link @click="login">LOG IN</el-link>
          </el-col>
        </el-row>
      </el-header>

      <el-header> </el-header>
      <el-header> </el-header>

      <el-container>
        <el-main>
          <div class="courses_bg">
            <h1 style="font-family: monaco; font-size: 30px">
              popular courses
            </h1>

            <el-row :gutter="20">
              <el-col :span="6">
                <el-card :body-style="{ padding: '20px' }">
                  <img src="../../assets/img/python.jpg" class="image" />
                  <div class="courses_txt" style="padding: 10px">
                    <span>courses</span>
                  </div>
                </el-card>
              </el-col>
              <el-col :span="6">
                <el-card :body-style="{ padding: '20px' }">
                  <img src="../../assets/img/python.jpg" class="image" />
                  <div class="courses_txt" style="padding: 10px">
                    <span>courses</span>
                  </div>
                </el-card>
              </el-col>
              <el-col :span="6">
                <el-card :body-style="{ padding: '20px' }">
                  <img src="../../assets/img/python.jpg" class="image" />
                  <div class="courses_txt" style="padding: 10px">
                    <span>courses</span>
                  </div>
                </el-card>
              </el-col>
              <el-col :span="6">
                <el-card :body-style="{ padding: '20px' }">
                  <img src="../../assets/img/python.jpg" class="image" />
                  <div class="courses_txt" style="padding: 10px">
                    <span>courses</span>
                  </div>
                </el-card>
              </el-col>
            </el-row>
          </div>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {
  methods: {
    home() {
      this.$router.push("Introduction");
    },
    login() {
      this.$router.push("Login");
    },
  },
};
</script>

<style lang="postcss" scoped>
.background {
  background-color: beige;
  background-image: url(../../assets/img/slider.jpg);
  background-size: 100%;
}
.courses_bg {
}
.el-header {
  text-align: right;
  line-height: 100px;
}
.el-main {
  height: 700px;
}
.el-aside {
  height: 700px;
}
.el-link {
  width: 120px;
  height: 50px;
  background-color: rgba(211, 193, 145, 0.315);
  font-size: 25px;
}

.image {
  width: 100%;
  display: block;
}

.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>
