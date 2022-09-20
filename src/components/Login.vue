<template>

<section>
    <div class="ui segment grey login-form">
        <h2 class="ui header">Station Login</h2>
        <form class="ui form">
            <div class="ui stacked segment">
                <div class="field">
                    <div class="ui left icon input big">
                        <i class="user icon"></i>
                        <input type="text" placeholder="User Name" />
                    </div>

                </div>
                <div class="field">
                    <div class="ui left icon input big">
                        <i class="lock icon"></i>
                        <input type="password" placeholder="Password"/>
                    </div>

                </div>
                <button class="ui button big blue fluid " >Login</button>

            </div>
        </form>
    </div>
    
</section>
    
</template>

<style scoped>
section{
    height: 100vh;
    background-color: #ececec;
    display: flex;
    align-items: center;
    justify-content: center;
}
.login-form{
    width: 450px;
}

</style>