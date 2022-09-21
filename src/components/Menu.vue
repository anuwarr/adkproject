<template>
    <section>
        <div class=" ui pointing menu menu-bar" >
             <div class="item">
    <img src="@/assets/img/adklogo.jpg">
  </div>
           <router-link class="item" to="/floor">Home</router-link>
          <router-link class="item" to="/inventory">
            Inventory
          </router-link>
  <a class="item">History</a>
  <div class="right menu">
    <div class="item">
      <div class="ui icon input">
        <input type="text" placeholder="Search...">
        <i class="search link icon"></i>
      </div>
    </div>
    <a class="ui item">
      Logout
    </a>
  </div>
            
        </div>
    </section>
</template>


<script>
export default {
   name:'Menu'
}
</script>

<style scoped>
.menu-bar{
    background-color:#34c6eb;
}
</style>