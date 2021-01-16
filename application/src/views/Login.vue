<template>
    <div class="login flex-container-colunm bounceInDown">
        <div class="box-login-superior">
            <form class="form-content">
                <h1 class="title-box-content">Log in</h1>
                <div class="form-input">
                    <input type="text" placeholder="username@email.com" />
                </div>
                <div class="form-input">
                    <input type="password" placeholder="password" />
                </div>
                <div class="form-check">
                    <a href="#" class="forgot">forgot</a>
                    <label for="c-remember">
                    <input type="checkbox" id="c-remenber" name="c-remember" /> Remember me</label>
                </div>
                <div class="form-button">
                    <button @click="login">Go</button>
                </div>
            </form>
        </div>
        <div class="box-auth-medias">
            <span>or connect</span>
        </div>
        <div class="box-login-inferior flex-container-inline">
            <a href="" class="btn btn-google">
                <svg>
                    <g>
                        <path class="st0" d="M0.5,8.3C0.4,4,4.1,0.1,8.4,0c2.2-0.2,4.3,0.7,6,2c-0.7,0.7-1.4,1.5-2.1,2.2c-1.5-0.9-3.2-1.6-4.9-1
                            C4.6,4.1,2.9,7.3,4,10c0.8,2.8,4.2,4.3,6.9,3.2c1.4-0.5,2.3-1.8,2.7-3.1c-1.6,0-3.2,0-4.8-0.1c0-0.9,0-1.9,0-2.8
                            c2.6,0,5.3,0,7.9,0c0.2,2.3-0.2,4.8-1.7,6.6c-2.1,2.6-5.9,3.4-8.9,2.4C2.8,15.1,0.5,11.8,0.5,8.3z"/>
                        <path class="st0" d="M21.9,4.7c0.8,0,1.6,0,2.4,0c0,0.8,0,1.6,0,2.4c0.8,0,1.6,0,2.4,0c0,0.8,0,1.6,0,2.4c-0.8,0-1.6,0-2.4,0
                            c0,0.8,0,1.6,0,2.4c-0.8,0-1.6,0-2.4,0c0-0.8,0-1.6,0-2.4c-0.8,0-1.6,0-2.4,0c0-0.8,0-1.6,0-2.4c0.8,0,1.6,0,2.4,0
                            C21.9,6.3,21.9,5.5,21.9,4.7z"/>
                    </g>
                </svg>
            </a>
            <a href="" class="btn btn-linkedin">
                <svg>
                    <g>
                        <g>
                            <path class="st0" d="M18.4,11.3v6.3h-3.7v-5.9c0-1.5-0.5-2.5-1.9-2.5c-1,0-1.6,0.7-1.9,1.3c-0.1,0.2-0.1,0.6-0.1,0.9v6.2H7.1
                                c0,0,0-10,0-11h3.7v1.6c0,0,0,0,0,0h0v0c0.5-0.8,1.4-1.8,3.3-1.8C16.5,6.3,18.4,7.9,18.4,11.3L18.4,11.3z M3.3,1.3
                                C2,1.3,1.2,2.1,1.2,3.2c0,1.1,0.8,1.9,2,1.9h0c1.3,0,2.1-0.8,2.1-1.9C5.3,2.1,4.6,1.3,3.3,1.3L3.3,1.3z M1.4,17.6h3.7v-11H1.4
                                V17.6z"/>
                        </g>
                    </g>
                </svg>
            </a>
            <a href="" class="btn btn-twitter">
                <svg>
                    <g>
                        <g>
                            <path class="st0" d="M20.5,2.6c-0.8,0.3-1.6,0.6-2.4,0.7c0.9-0.5,1.5-1.3,1.8-2.3c-0.8,0.5-1.7,0.8-2.7,1
                                c-0.8-0.8-1.9-1.3-3.1-1.3c-2.3,0-4.2,1.9-4.2,4.2c0,0.3,0,0.7,0.1,1C6.6,5.6,3.5,4,1.4,1.4C1.1,2,0.9,2.8,0.9,3.5
                                C0.9,5,1.6,6.3,2.7,7C2,7,1.4,6.8,0.8,6.5c0,0,0,0,0,0.1c0,2,1.5,3.7,3.4,4.1c-0.4,0.1-0.7,0.1-1.1,0.1c-0.3,0-0.5,0-0.8-0.1
                                c0.5,1.7,2.1,2.9,3.9,2.9C4.8,14.8,3,15.5,1,15.5c-0.3,0-0.7,0-1-0.1c1.9,1.2,4.1,1.9,6.4,1.9c7.7,0,12-6.4,12-12
                                c0-0.2,0-0.4,0-0.5C19.2,4.2,19.9,3.5,20.5,2.6L20.5,2.6z"/>
                        </g>
                    </g>
                </svg>
            </a>
        </div>
        <div class="box-new-account-mobile hidden-desktop">
            <router-link to="/sign-up"><span>create <strong>new</strong> account</span></router-link>
        </div>
        <div class="link-new-account hidden-mobile">
            <router-link to="/sign-up"><span>create <strong>new</strong> account</span></router-link>
        </div>
    </div>
</template>

<script>
export default {
    name: 'login',
    data() {
        return {};
    },
    methods: {
        login: function() {
            this.$router.replace('dashboard');
        }
    }
};
</script>

<style scoped>
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body, html{
    width: 100%;
    height: 100vh;
}

a{
    text-decoration: none;
}

h1{
    color: #161616;
    font-size: 1.8rem;
}

#app{
    background: #0043CE!important;
}

button{
    cursor: pointer;
}

input, button{
    outline: none!important;
}

.flex-container-colunm{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.flex-container-inline{
    display: inline-flex;
    justify-content: center;
    align-items: center;
}

.login{
    width: 320px;
    height: auto;
    position: relative;
    margin: 0 auto;
    top: 60px;
    z-index: 9999;
}

@media only screen and (max-width: 780px){

    .login{
        width: 100%!important;
        height: 100vh!important;
        padding: 0;
        margin: 0;
        overflow: hidden!important;
        bottom: 0;
        top: 0;
    }

    .box-login-superior{
        height: 70%!important;
        border-radius: 0!important;
    }

    .box-auth-medias{
        width: 100%;
        height: 10%;
        min-height: 10%;
    }

    .box-login-inferior{
        height: 20%!important;
        border-radius: 0!important;
    }

    .box-new-account-mobile{
        width: 100%;
        height: 10%!important;
        background-color: #161616;
        margin-top: -1px!important;
    }

    .box-new-account-mobile span{
        color: #fff;
    }

    .hidden-mobile{
        display: none;
    }
    
}

@media only screen and (min-width: 780px){

    .hidden-desktop{
        display: none;
    }
}

.box-login-superior{
    width: 100%;
    padding: 20px;
    background-color: #fff;
    border-radius: 10px 10px 0 0;
    box-shadow: 1px -1px 20px rgba(0,0,0,.15);
}

.box-auth-medias{
    width: 100%;
    height: 40px;
    min-height: 40px;
    display: -webkit-flex;
    display: flex;
    -webkit-align-items: flex-end;
    align-items: flex-end;
    -webkit-justify-content: center;
    justify-content: center;
    background-color: #161616;
    margin-bottom: -2px;
}

.box-auth-medias span{
    color: #fff;
}

.box-login-inferior{
    width: 100%;
    padding: 20px;
    background-color: #161616;
    border-radius: 0 0 10px 10px;
    box-shadow: -1px 10px 15px rgba(0,0,0,.30);
    margin-top: -1px!important;
}

.title-box-content{
    margin-bottom: 10px;
}

.form-input input{
    width: 270px;
    padding: 10px 15px;
    border-radius: 30px;
    border: 1px solid rgb(177, 177, 177);
    margin: 10px 0;
}

.form-input input:focus{
    padding: 15px 20px;
    transition: .4s;
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
}

.form-button button{
    margin: 30px 0 10px 0;
    background-color: #002d9c;
    padding: 10px 30px;
    color: #fff;
    font-weight: 600;
    text-transform: uppercase;
    border: none;
    border-bottom: 4px solid #001D6C!important;
    border-radius: 5px;
}

.form-button button:hover{
    background-color: #022680;
}

.btn{
    width: 75px;
    height: 37px;
    border-radius: 5px;
    margin: 5px;
}

.btn a{
    color: #fff;
}

.st0{fill:#FFFFFF;}

.btn-google{
    padding: 9px 25px;
    background-color: #da3e2f;
    border-bottom: 3px solid #bb2c1f;
}

.btn-google:hover{
    background-color: #c73629;
}

.btn-linkedin{
    padding: 7px 28px;
    background-color: #007ab9;
    border-bottom: 3px solid #025781;
}

.btn-linkedin:hover{
    background-color: #0370a7;
}

.btn-twitter{
    padding: 8px 28px;
    background-color: #55acee;
    border-bottom: 3px solid #3784be;
}

.btn-twitter:hover{
    background-color: #4795d1;
}

.form-check{
    width: 100%;
    padding-bottom: 20px;
}

.form-check label{
    position: relative;
    float: left;
    margin-left: 10px;
}

.form-check a{
    position: relative;
    float: right;
    margin-right: 15px;
}

.forgot{
    color: #002d9c;
}

.link-new-account{
    margin-top: 10px;
}

.hidden-mobile span{
    color: #002d9c!important;
}

/** animation - box login **/
.bounceInDown {
  -webkit-animation-name: bounceInDown;
  animation-name: bounceInDown;
  -webkit-animation-duration: 1s;
  animation-duration: 1s;
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
  }
  @-webkit-keyframes bounceInDown {
  0%, 60%, 75%, 90%, 100% {
  -webkit-transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
  transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
  }
  
  0% {
  opacity: 0;
  -webkit-transform: translate3d(0, -3000px, 0);
  transform: translate3d(0, -3000px, 0);
  }
  
  60% {
  opacity: 1;
  -webkit-transform: translate3d(0, 25px, 0);
  transform: translate3d(0, 25px, 0);
  }
  
  75% {
  -webkit-transform: translate3d(0, -10px, 0);
  transform: translate3d(0, -10px, 0);
  }
  
  90% {
  -webkit-transform: translate3d(0, 5px, 0);
  transform: translate3d(0, 5px, 0);
  }
  
  100% {
  -webkit-transform: none;
  transform: none;
  }
  }
  
  @keyframes bounceInDown {
  0%, 60%, 75%, 90%, 100% {
  -webkit-transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
  transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
  }
  
  0% {
  opacity: 0;
  -webkit-transform: translate3d(0, -3000px, 0);
  transform: translate3d(0, -3000px, 0);
  }
  
  60% {
  opacity: 1;
  -webkit-transform: translate3d(0, 25px, 0);
  transform: translate3d(0, 25px, 0);
  }
  
  75% {
  -webkit-transform: translate3d(0, -10px, 0);
  transform: translate3d(0, -10px, 0);
  }
  
  90% {
  -webkit-transform: translate3d(0, 5px, 0);
  transform: translate3d(0, 5px, 0);
  }
  
  100% {
  -webkit-transform: none;
  transform: none;
  }
  } 

</style>