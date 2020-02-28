<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/profile">Profile</router-link> |
      <router-link to="/about">About</router-link>

    </div>
    <router-view/> -->
    <div class="container">
      <div class="row header mb-2 p-3">
        <div class="col-lg-12">
          <h2>What do i do today?</h2>
        </div>
      </div>
      <div class="row content">
        <div class="col-lg-12">
          <div class="pekerjaan-rumah">
            <div class="row">
              <div v-for="tugasSaya in tugas" v-bind:key="tugasSaya.idTugas" class="mb-3 tugas col-lg-12 text-left">
                <div class="form-check">
                  <ItemTugas v-bind:tugasSaya="tugasSaya"/>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import ItemTugas from "./components/ItemTugas.vue"
export default {
  name:'app',
  data: function(){
    return {
      tugas: [
      {
        idTugas:1,
        namaTugas:'membersihkan toilet',
        isDone: false
      },
      {
        idTugas:2,
        namaTugas:'membersihkan kamar',
        isDone: false
      },
      {
        idTugas:3,
        namaTugas:'membersihkan dapur',
        isDone: false
      }
    ]
    }
  },
  components:{
    ItemTugas
  }
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 50px;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.header{
  background: #1abc9c;
}
.header h2 {
  margin: 0;
}
.tugas .item{
  font-size: 18px;
  text-align: left;
}
.item-complete{
  color: #1abc9c;
}
</style>
