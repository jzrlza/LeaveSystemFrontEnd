<template>
 
    <!--Navbar-->
    <navbar placement="top" type="default" class="the-nav">
  <!-- Brand as slot -->
  <router-link slot="brand" to="/admin-users" title="Home" class="navbar-brand">Leave Request System [Administrator]</router-link>
  <!-- You can use dropdown component -->
  
  <li class="dropdown">
    <router-link to="/admin-users">Manage Users</router-link>
  </li>
 
  <!-- Or normal bootstrap style -->
  <li class="dropdown">
    <router-link to="/admin-print-report">Print Statistic Report</router-link>
  </li>

  <li class="dropdown">
    <router-link to="/">Logout</router-link>
  </li>

  <li class="dropdown">
    <a id="current_user">-username_admin-</a>
  </li>

</navbar>
    <!--/.Navbar-->
  
</template>

<script>
import Navbar from '@/components/Navbar'
import NavbarItem from '@/components/NavbarItem'
import NavbarItemDropdown from '@/components/NavbarItemDropdown'
import NavbarNav from '@/components/NavbarNav'
import NavbarCollapse from '@/components/NavbarCollapse'

export default {
  name: 'AdminUsers',
  components: {
    Navbar,
    NavbarItem,
    NavbarItemDropdown,
    NavbarNav,
    NavbarCollapse
  },
  data () {
    return {
      msg: 'ADMIN USER PLACEHOLDER'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .navbar .dropdown-menu a:hover {
    color: red !important;
  }
  .navbar-brand:hover{
    color: green;
  }
  .the-nav {
    background-color: teal;
  }
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  color: #42b983;
  display: inline-block;
  margin: 0 10px;
}
a, router-link , .navbar-brand{
  color: #42b983;
}
.navbar-item {
  color: #42b983;
}
#current_user {
  color: grey;
}
</style>
