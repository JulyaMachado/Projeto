<template>
    <div class="login flex-container">
        <form>
            <h1 title="title-box-content">Log in</h1>
            <input type="text" placeholder="username@email.com" />
            <input type="password" placeholder="Password" />
            <button type="submit">Go</button>
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

</style>