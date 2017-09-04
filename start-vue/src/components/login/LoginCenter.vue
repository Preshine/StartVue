<<template>
  <img src="LoginCenterBg.jpg" class="login-background" >
  <div class="login-form-wrapper">
      <form class="main-form login-form" method="post" >
          <div class="login-logo-warpper" >
              <img src="login-logo.png" class="login-logo" >
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
.login-background {
    position: fixed;
    height: 100%;
    width: 100%;
    z-index: -100;
}
.login-form-wrapper {
    padding-top: 150px;
}
.main-form, .main-form * {
    box-sizing: border-box;
}
.main-form {
    box-sizing: border-box;
    width: 360px;
    max-width: 95%;
    margin: 0 auto;
}
.login-form {
    background-color: #fff;
    padding: 40px;
}
.login-logo-wrapper {
    text-align: center;
}
.main-form * {
    display: inline-block;
}
.login-form .login-form-form-item {
    display: block;
    border: none;
    border-radius: 3px;
    background-color: #f5f4f3;
    padding: 10px 14px;
    margin: 0 auto 15px;
}
.login-form .login-form-item .login-email-icon {
    margin-bottom: 3px;
}
img {
    vertical-align: middle;
}
img {
    border: 0;
}
.login-form .login-form-item .login-form-input {
    border: none;
    background-color: #f5f4f3;
    width: 80%;
    margin-left: 12px;
}
.login-form .login-form-item .login-password-icon {
    margin: 0 3px 3px;
}
.login-form .login-form-item.captcha-item {
    width: 60%;
    float: left;
}
.login-form .login-form-item.captcha-item .captcha-input {
    margin: 0;
}
.login-form .login-button {
    display: block;
    width: 100%;
    font-size: 18px;
    background: #e4e40c;
    border: none;
    border-radius: 3px;
    padding: 10px;
    margin-bottom: 10px;
}
.forget-password-link, .register-link {
    display: block;
}
</style>

