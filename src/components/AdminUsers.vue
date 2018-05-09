<template>
 <div>
  <navbar></navbar>

  <user-manage></user-manage>
 </div>
  
</template>

<script>
import Navbar from '@/components/AdminNavBar'
import UserManage from '@/components/UserManager'

export default {
  name: 'AdminUsers',
  components: {
    Navbar,
    UserManage
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
  
</style>
