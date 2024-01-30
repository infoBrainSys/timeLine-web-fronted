<script>
  import '@/assets/menu.less'

  export default {
    data(){
      return{
        isLogin:true,
        loginData:{
          username: '',
          password: ''
        },
        RegisterData:{
          username: '',
          password: ''
        }
      }
    },
    methods:{
      // TODO 处理登录信息和提交动作
      Login(){

      },
      //  TODO 处理注册信息和提交动作
      Register(){

      },
      // 切换登录和注册表单
      toggleForm(){
        this.isLogin = !this.isLogin
      }
    }
  }
</script>

<template>
  <div ref="menuBox" class="menu-box">

<!--    首页 emoji 设计-->
    <div class="emoji-box">
      <a href="#">
        <i class="fa-solid fa-face-smile"></i>
        <i class="fa-solid fa-face-grin-wink"></i>
      </a>
    </div>

    <div ref="formCard" class="form-card">
      <form v-if="isLogin" @submit.prevent="Login" class="login-form" action="#" method="get">
        <div class="login-form-title">
          <span>Login</span>
        </div>
        <input type="text" name="username" id="username" placeholder="username">
        <input type="password" name="password" id="password" placeholder="password">
        <button type="submit"><span>Login</span></button>
        <p>Don't have an account? <a @click="toggleForm">Register>></a></p>
      </form>

      <form v-else @submit.prevent="Register" class="register-form" action="#" method="get">
        <div class="register-form-title">
          <span>Register</span>
        </div>
        <input type="text" name="username" id="username" placeholder="username">
        <input type="password" name="password" id="password" placeholder="password">
        <button type="submit"><span>Register</span></button>
        <p>Already have an account? <a @click="toggleForm">Login>></a></p>
      </form>
    </div>
  </div>
</template>