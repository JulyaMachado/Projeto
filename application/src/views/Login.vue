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

a{
    text-decoration: none;
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
    width: 75px;
    height: 37px;
    border-radius: 5px;
}

.btn a{
    color: #fff;
}

.st0{fill:#FFFFFF;}

.btn-google{
    padding: 9px 25px;
    background-color: #EA4335;
    border-bottom: 3px solid #bb2c1f;
}

.btn-linkedin{
    padding: 7px 28px;
    background-color: #007ab9;
    border-bottom: 3px solid #025781;
}

.btn-twitter{
    padding: 8px 28px;
    background-color: #55acee;
    border-bottom: 3px solid #3e90cf;
}

</style>