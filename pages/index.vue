<template>
  <div>
    <div class="searchBarBox">
      <div class="searchBar">
        <div class="searchBarInput">
          <img src="~/assets/img/loupe.png" alt="" class="searchLogo">
          <input type="text" class="searchText" placeholder="Search...">
        </div>
        <div class="searchBtn">GO</div>
      </div>
    </div>
    <div class="resultList">
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data: function () {
    return {
    }
  },
}
</script>

<style scoped>

.searchBarBox {
  width: 100vw;
  display: flex;
  justify-content: center;
}

.searchBar {
  background-color: #56BDF5;
  width: 400px;
  height: 50px;
  border-radius: 40px; 
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: white;
  margin-top: 100px;
}

.searchBarInput {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: left;
}

.searchLogo {
  height: 40%;
  margin-left: 20px;
}

.searchText {
  margin-left: 20px;
  background: none;
  border: none;
  outline: none;
  color: white;
  width: 263px;
}

.searchBtn {
  height: 35px;
  color: #56BDF5;
  background-color: white;
  border-radius: 30px;
  padding: 2px 20px;
  margin-right: 5px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.resultList {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  width: 90%;
  margin: 0px 5%;
}
</style>
