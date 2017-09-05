<template>
    <div class="login">
        <img src="./LoginCenterBg.jpg" class="login-background">
        <div class="login-form-wrapper">
            <form class="main-form login-form" method="post">
                <div class="login-logo-wrapper">
                    <img src="./login-logo.png" class="login-logo">
                </div>
                <div class="login-form-item">
                    <img src="./email.png" class="login-email-icon">
                    <input type="text" class="login-form-input" name="email" placeholder="邮箱">
                </div>
                <div class="login-form-item">
                    <img src="./password.png" class="login-password-icon">
                    <input type="password" class="login-form-input" name="password" placeholder="密码">
                </div>
                <div class="login-form-item captcha-item">
                    <input type="text" class="login-form-input captcha-input" name="captcha" placeholder="验证码">
                </div>
                <img id="captcha-img" alt="验证码" src="./captcha.png">
                <button class="login-button" type="button" @click="login('Preshine')">登录</button>
                <div class="forget-password-link">
                    <a href="javascript:void(0);">忘记密码</a>
                </div>
                <div class="register-link">
                    <a href="javascript:void(0);">立即注册</a>
                </div>

            </form>
        </div>
        <hello ref="hello" ></hello>
    </div>
</template>

<script>
import hello from '../../Hello'
export default {
    name: 'login',
    data() {
        return {
            msg: 'Welcome to Your Vue.js App'
        }
    },
    methods: {
        login(username) {
            console.log(username);
            debugger;
            this.$refs.hello.show();
        }
    },
    components: {
        hello
    }
}
</script>

<<style scoped>
.login {
    width: 100%;
    height:100%;
}

.login-background {
    position: fixed;
    height: 100%;
    width: 100%;
    z-index: -100;
}
.login-form-wrapper {
    padding-top: 150px;
    filter:alpha(opacity=80);
    -moz-opacity:0.80;
    -khtml-opacity:0.80;
    opacity:0.80;
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
.login-logo-wrapper .login-logo {
    width: 65%;
    height: auto;
    margin-top: -5px;
    margin-bottom: 25px;
}
.main-form * {
    display: inline-block;
}
.login-form .login-form-item {
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
input {
    outline: none;
}
input:-webkit-autofill, 
 textarea:-webkit-autofill, 
 select:-webkit-autofill { 
       -webkit-box-shadow: 0 0 0 1000px #f5f4f3 inset; 
}
 input[type=text]:focus, input[type=password]:focus, textarea:focus {
      -webkit-box-shadow: 0 0 0 1000px #f5f4f3 inset; 
}
button {
    cursor: pointer;
}
.login-button:hover {
    background: #FFD700;
}
.forget-password-link, .register-link {
    display: block;
}
.forget-password-link a {
    float: left;
    margin-bottom: 20px;
    color: #333;
}
.register-link a {
    float: right;
    margin-bottom: 20px;
    color: #333
}
</style>

