<template>
  <div id="app">
    <div class="container">
      <div class="row header mb-5 p-3">
        <div class="col-lg-12">
          <h2>
            What i do today ?
          </h2>
        </div>
      </div>
      <div class="row content">
        <div class="col-lg-12">
         <div class="pekerjaan-rumah">
            <div v-for="tugasSaya in tugas" v-bind:key="tugasSaya.id" class="mb-4 tugas col-lg-12 text-left">
            <div class="form-check">
              <input class="form-check-input" onclick="" type="checkbox" value="" id="defaultCheck1">
              <label class="form-check-label item" for="defaultCheck1">
               {{ tugasSaya.namaTugas }}
              </label>
            </div>
          </div>
         </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'app',
    data: function () {
      return {
        tugas: [
          {
            id: 1,
            namaTugas: 'Membersihkan Toilet',
            isDone: false
          },
          {
            id: 2,
            namaTugas: 'Makan',
            isDone: false
          },
          {
            id: 3,
            namaTugas: 'Ngoding',
            isDone: false
          },
           {
            id: 4,
            namaTugas: 'Menggambar',
            isDone: false
          }
        ]
      }
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
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

  .header {
    background: #42b983;
  }

  .header h2 {
    margin: 0;
  }

  .tugas item {
    font-size: 20px;
  }
</style>