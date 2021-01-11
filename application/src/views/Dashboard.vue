<template>
  <div class="dashboard">
    <header class="flex-container-inline">
        <div class="box-left">
            <p>STOP <strong>Bug</strong></p>
        </div>
        <div class="box-center">
            center
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
}

header{
    padding: 0!important;
    margin: 0!important;
    width: 100%;
    height: 60px;
    background-color: #161616;
    color: #ffffff;
}

.box-left{
    width: 20%;
}

.box-center{
    width: 60%;
}

.box-right{
    width: 20%;
}

.btn-logout{
    width: 60px;
    height: 60px;
    background-color: #161616;
    position: relative;
    float: right;
    cursor: pointer;
}

.st0{fill:#FFFFFF;}

</style>