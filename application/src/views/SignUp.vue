<template>
    <div class="sign-up">
        <div class="box-login-superior">
            <form class="form-content">
                <h1 class="title-box-content">New account</h1>
                <div class="form-input">
                    <input type="text" placeholder="username@email.com" v-model="email" />
                </div>
                <div class="form-input">
                    <input type="password" placeholder="password" v-model="senha" />
                </div>
                <div class="form-input">
                    <input type="password" placeholder="confirm password" v-model="senha" />
                </div>
                <div class="form-button">
                    <button @click="sign-up">Register</button>
                </div>
            </form>
        </div>
        <div class="box-login-inferior">
            <a @click="login"><span class="back">⬅ back</span></a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'sign-up',
    data() {
        return {
            email: '',
            senha: '',
        };
    },
    methods: {
        login: function() {
            this.$router.replace('/');
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

.title-box-content{
    margin-bottom: 10px;
}

.flex-container-inline{
    display: inline-flex;
    justify-content: center;
    align-items: center;
}

.sign-up{
    width: 320px;
    height: auto;
    position: relative;
    margin: 0 auto;
    top: 40px;
    z-index: 999;;
}

.box-login-superior{
    width: 100%;
    padding: 20px;
    background-color: #fff;
    border-radius: 10px 10px 0 0;
    box-shadow: 1px 3px 20px rgba(0,0,0,.15);
}

.box-login-inferior{
    width: 100%;
    padding: 20px;
    background-color: #161616;
    border-radius: 0 0 10px 10px;
    box-shadow: 1px 2px 15px rgba(0,0,0,.30);
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
    margin: 20px 0 10px 0;
    background-color: #002d9c;
    padding: 10px 30px;
    color: #fff;
    font-weight: 600;
    text-transform: uppercase;
    border: none;
    border-bottom: 3px solid #001D6C!important;
    border-radius: 5px;
}

.form-button button:hover{
    background-color: #022680;
}

.back{
    color: #fff;
    cursor: pointer!important;
}
</style>