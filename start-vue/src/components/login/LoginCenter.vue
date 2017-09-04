<<template>
  <img src="LoginCenterBg.jpg" class="login-background" >
  <div class="login-form-wrapper">
      <form class="main-form login-form" method="post" >
          <div class="login-logo-warpper" >
              <img src="" class="login-logo" >
          </div>
          <div class="login-form-item" >
              <img src="Email.png" class="login-email-icon" >
              <input type="text" class="login-form-input" name="email" placeholder="邮箱" value>
          </div>
          <div class="login-form-item" >
              <img src="" class="login-password-icon" >
              <input type="password" class="login-form-input" name="password" placeholder="密码" value>
          </div>
          <div class="login-form-item captcha-item" >
              <input type="text" class="login-form-input captcha-input" name="captcha" placeholder="验证码" >
          </div>
          <img id="captcha-img" alt="验证码" src="captcha.png" >
          <button class="login-button" type="submit" >登录</button>
          <div class="forget-password-link"><a href="javascript:void(0);">忘记密码</a></div>
          <div class="register-link"><a href="javascript:void(0);">立即注册</a></div>

      </form>
  </div>
</template>

<<script>
export default {
  
}
</script>

<<style scoped>

</style>

