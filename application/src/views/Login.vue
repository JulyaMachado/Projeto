<template>
    <div class="login flex-container">
        <form class="form-content">
            <h1 title="title-box-content">Log in</h1>
            <div class="form-input">
                <!--<label>Username</label><br />-->
                <input type="text" placeholder="username@email.com" />
            </div>
            <div class="form-input">
                <!--<label>Password</label><br />-->
                <input type="password" placeholder="Password" />
            </div>
            <div class="form-button">
                <button type="submit">Go</button>
            </div>
        </form>
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

body{
    width: 100%;
    height: 100vh;
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
    padding: 20px;
    background-color: #fff;
    border-radius: 20px;
    box-shadow: 1px 1px 15px rgba(0,0,0,.25);
}

.form-input label{
    text-align: left;
    position: relative;
    float: left;
    margin-top: 15px;
    font-size: .8rem;
    font-weight: 600;
}

.form-input input{
    padding: 10px 15px;
    border-radius: 30px;
    border: 1px solid #999;
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
}


</style>