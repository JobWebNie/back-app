<template>
    <div class="n_toast">
        <div class="container">
        <div class="header-name">
            注册
        </div>
        <div style="line-height: 45px;
        font-size: 45px;color:#409eff;text-align: center;margin: 50px auto 60px">
            LOGO
        </div>
        <div class="form-body">
            <div class="input-inner">
                <input type="text" placeholder="请输入手机号">
            </div>
            <div class="input-inner" style="display:flex;overflow: hidden;">
                <input style="width:56%" type="text" placeholder="请输入验证码">
                <div class="btn-code" id="btn-code">
                    获取验证码
                </div>
            </div>
            <div class="input-btn">
                确认注册
            </div>
            <div class="cheack-agreement">
                <span class="check-btn ischeck"></span>
                同意用户协议
            </div>
        </div>
    </div>
    </div>
</template>
<script>
    export default {
        name:'NToast',
        props:{
           
        }
    }
</script>

<style>
/* div.n_toast
    display inline-block
    line-height 1px
    font-size 16px
    width 100%
    height 36px */

.container{
    display: flex;
    flex-direction: column;
    width: 100vw;
    height: 100vh;
}
.header-name{
    width: 100%;
    font-size: 17px;
    padding: 0 10px;
    color: #2c8fff;
    box-sizing: border-box;
    margin-top: 14.5px;
    text-align: center;
}
.form-body{
    width: 277.5px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
}
.input-inner{
    border-radius: 17px;
    height: 34px;
    font-size: 13px;
    margin-bottom: 15px;
    border:1px solid #2c8fff;
}
.input-inner input{
    -webkit-appearance: none;
    padding: 0;
    width: 100%;
    color: #666666;
    text-indent: 16px;
    height: 34px;
    border: none;
    background-color: inherit;
    outline: none;
}
.input-btn{
    border-radius: 17px;
    height: 34px;
    font-size: 13px;
    border: 1px solid #2c8fff;
    color: #fff;
    padding: 7px 0;
    text-align: center;
    margin-top: 10px;
    line-height: 17px;
    box-sizing: border-box;
    background-color: #2c8fff;
    box-shadow: 0 2px 10px #2c8fff;
}
.btn-code{
    border-top-right-radius: 17px;
    border-bottom-right-radius: 17px;
    height: 34px;
    font-size: 13px;
    border: 1px solid #2c8fff;
    color: #fff;
    padding: 7px 0;
    text-align: center;
    line-height: 17px;
    box-sizing: border-box;
    background-color: #2c8fff;
    box-shadow: 0 2px 10px #2c8fff;
    width:44%;
}
.cheack-agreement{
    font-size: 13px;
    padding: 0 10px;
    color: #666666;
    box-sizing: border-box;
    margin-top: 14.5px;
    text-align: center;
}
.check-btn{
    border: 1px solid #dcdfe6;
    border-radius: 1px;
    margin-right: 8px;
    width: 12px;
    height: 12px;
    background-color: #fff;
    position: relative;
    cursor: pointer;
    display: inline-block;
    box-sizing: border-box;
}

.check-btn:after{
    width: 8px;
    height: 8px;
    border-radius: 1px;
    background-color: #dcdfe6;
    content: "";
    position: absolute;
    left: 10%;
    top: 10%;
}
.ischeck.check-btn{
    border-color: #409eff;
}
.ischeck.check-btn:after{
    background-color: #409eff;
}
</style>