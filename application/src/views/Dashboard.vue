<template>
  <div class="dashboard">
    <div class="box-total">
            <span>don't waste more time with bug</span>
        </div>
    <header class="flex-container-inline">
        
        <div class="box-left">
            <p>STOP <strong>Bug</strong></p>
        </div>
        <div class="box-center">
            <form>
                <div class="form-search">
                    <input type="text" placeholder="Search solution..." />
                </div>
            </form>
        </div>
        <div class="box-right">
            <div class="btn-logout">
                <svg>
                    <g>
                        <g>
                            <path class="st0" d="M9,16.6H2.3c-0.4,0-0.8-0.3-0.8-0.8V2.3c0-0.4,0.3-0.8,0.8-0.8H9c0.4,0,0.8-0.3,0.8-0.8S9.5,0,9,0H2.3
                                C1,0,0,1,0,2.3v13.6c0,1.2,1,2.3,2.3,2.3H9c0.4,0,0.8-0.3,0.8-0.8S9.5,16.6,9,16.6z"/>
                        </g>
                    </g>
                    <g>
                        <g>
                            <path class="st0" d="M17.9,8.5L13.3,4c-0.3-0.3-0.8-0.3-1.1,0s-0.3,0.8,0,1.1l3.3,3.2H6.8C6.4,8.3,6,8.6,6,9
                                c0,0.4,0.3,0.8,0.8,0.8h8.8L12.3,13c-0.3,0.3-0.3,0.8,0,1.1c0.1,0.1,0.3,0.2,0.5,0.2c0.2,0,0.4-0.1,0.5-0.2l4.6-4.5
                                c0.1-0.1,0.2-0.3,0.2-0.5C18.1,8.8,18.1,8.6,17.9,8.5z"/>
                        </g>
                    </g>
                </svg>
            </div>
        </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "dashboard",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style scoped>
a{
    text-decoration: none!important;
}

.flex-container-inline{
    display: inline-flex;
    overflow-x: hidden;
}

header{
    padding: 0!important;
    margin: 0!important;
    width: 100%;
    height: 60px;
    background-color: #161616;
    box-shadow: 1px 5px 10px rgba(0, 0, 0, .5);
    color: #ffffff;
    overflow: hidden;
}

.box-total{
    display: block;
    background-color: #000;
    width: 100%;
    height: 30px;
    color: #fff;
}

.box-total span{
    font-size: .65rem;
    letter-spacing: 1px;
    position: relative;
    top: 5px;
    font-weight: 200;
    text-transform: uppercase;
}

.box-left{
    width: 20%;
    height: 60px;
}

.box-left p{
    margin: 20px 23px;
    position: relative;
    float: left;
}

.box-center{
    width: 60%;
    height: 60px;
}

.box-center input{
    width: 70%;
    padding: 10px 15px;
    position: relative;
    margin: 10px 0;
    background-color: #161616;
    border: 1px solid rgba(255, 255, 255, .3);
    border-radius: 30px;
    color: #fff!important;
    outline: none!important;
}

.box-center input:focus{
    padding: 10px 18px;
    transition: .4s;
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
}

.box-right{
    width: 20%;
    height: 60px;
}

.btn-logout{
    width: 60px;
    height: 60px;    
    background-color: #161616;
    position: relative;
    float: right;
    cursor: pointer;
}

.btn-logout:hover{
    background-color: #252525;
    transition: .7s;
    -webkit-transition: .7s;
    -moz-transition: .7s;
    -o-transition: .7s;
}

.btn-logout svg{
    margin: 20px 23px;
}

.st0{fill:#FFFFFF;}

</style>