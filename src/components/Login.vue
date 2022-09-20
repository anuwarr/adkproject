<template>

<section>
    <div class="ui segment grey login-form">
        <h2 class="ui header">Station Login</h2>
        <form class="ui form">
            <div class="ui stacked segment">
                <div class="field">
                    <div class="ui left icon input big">
                        <i class="user icon"></i>
                        <input type="text" v-model="email" placeholder="User Name" />
                    </div>

                </div>
                <div class="field">
                    <div class="ui left icon input big">
                        <i class="lock icon"></i>
                        <input type="password" v-model="password" placeholder="Password"/>
                    </div>

                </div>
                <button class="ui button big blue fluid "  @click="login">Login</button>

            </div>
        </form>
    </div>
    
</section>
    
</template>

<script>
import axios from 'axios'
export default {
    name: 'Login',
    data() {
        return {
            email:'',
            password:'',
        }
    },
    methods:{
        async login(e){
            e.preventDefault();

            const result = await axios.get(
                `http://localhost:3000/users?email=${this.email}&password=${this.password}`
             

            )
            if (result.status == 200 && result.data.length>0) {

                localStorage.setItem("user-info",JSON.stringify(result.data[0]))
                this.$router.push({path:'/about'})
            }
          



              
            
            
        }

        

    
    }
    
    
}
</script>

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