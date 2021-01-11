<template>
    <div class="login flex-container">
        <div class="box-login-superior">
            <form class="form-content">
                <h1 class="title-box-content">Log in</h1>
                <div class="form-input">
                    <!--<label>Username</label><br />-->
                    <input type="text" placeholder="username@email.com" />
                </div>
                <div class="form-input">
                    <!--<label>Password</label><br />-->
                    <input type="password" placeholder="password" />
                </div>
                <div class="form-button">
                    <button type="submit">Go</button>
                </div>
            </form>
        </div>
        <div class="box-login-inferior flex-container">
            <div class="btn">
                <a href="" class="btn-google">Google</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'login',
    data() {
        return {};
    },
    methods: {}
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

#app{
    background: #0043CE!important;
}

input, button{
    outline: none!important;
}

.flex-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.login{
    width: 350px;
    height: auto;
    position: relative;
    margin: 0 auto;
}

.box-login-superior{
    width: 100%;
    padding: 20px;
    background-color: #fff;
    border-radius: 10px 10px 0 0;
    box-shadow: 1px 1px 15px rgba(0,0,0,.15);
}

.box-login-inferior{
    width: 100%;
    padding: 20px;
    background-color: rgba(0,17,65, .65);
    border-radius: 0 0 10px 10px;
    box-shadow: 1px 1px 15px rgba(0,0,0,.15);
}

.title-box-content{
    margin-bottom: 10px;
}

.form-input label{
    text-align: left;
    position: relative;
    float: left;  
    font-size: .8rem;
    font-weight: 600;
}

.form-input input{
    width: 250px;
    padding: 10px 15px;
    border-radius: 30px;
    border: 1px solid #999;
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
    margin-top: 15px;
    background-color: #002d9c;
    padding: 10px 30px;
    color: #fff;
    font-weight: 600;
    text-transform: uppercase;
    border: none;
    border-bottom: 3px solid rgba(15,98,254, .75)!important;
    border-radius: 5px;
}

.btn{
    width: 250px;
    padding: 10px;
    background-color: red;
}

</style>