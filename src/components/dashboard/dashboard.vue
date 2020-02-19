<template>
  <div id="dashboard">
    <h1>Информация / Отладка</h1>
    <ul>
      <li v-for="(zv, indx) in zv_list" :key=indx>
        id: {{ zv.id }} name: {{ zv.name }} os_id: {{ zv.os_id }}
      </li>
    </ul>
  </div>
</template>

<script>
  import axios from 'axios';

  export default {
    data () {
      return {
        zv_list: []
      }
    },
    created () {
      axios.get('/0/nss_type_zv.json')
        .then(res => {
          console.log(res)
          this.zv_list = res.data

          // const zv_list = []
          // for (let key in data) {
          //   const user = data[key]
          //   user.id = key
          //   users.push(user)
          // }
          // console.log(users)
          // this.email = users[0].email
        })
        .catch(error => console.log(error))
    }
  }
</script>

<style scoped>
  h1, p {
    text-align: center;
  }

  p {
    color: red;
  }
</style>