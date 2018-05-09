<template>
 
    <!--Navbar-->
    <navbar placement="top" type="default" class="the-nav">
  <!-- Brand as slot -->
  <router-link slot="brand" to="/sub-profile" title="Home" class="navbar-brand">Leave Request System [Subordinate]</router-link>
  <!-- You can use dropdown component -->
  
  <li class="dropdown">
    <router-link to="/sub-profile">Edit Profile</router-link>
  </li>

  <li class="dropdown">
    <router-link to="/sub-accept-tasks">Accept Tasks</router-link>
  </li>

  <li class="dropdown">
    <router-link to="/sub-accept-requests">Accept Substitude Requests</router-link>
  </li>

  <li class="dropdown">
    <router-link to="/sub-check">Check</router-link>
  </li>

  <li class="dropdown">
    <router-link to="/">Logout</router-link>
  </li>

  <li class="dropdown">
    <a id="current_user">-username_sub-</a>
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
  name: 'SubProfile',
  components: {
    Navbar,
    NavbarItem,
    NavbarItemDropdown,
    NavbarNav,
    NavbarCollapse
  },
  data () {
    return {
      msg: 'SUB USER PLACEHOLDER'
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
