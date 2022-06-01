<template>
  <div>
      <div class="card">
          <img :src="require(`~/assets/img/${link}`)" alt="" class="profile">
          <p class="name">{{name}}</p>
          <p class="job">{{job}}</p>
      </div>
  </div>
</template>

<script>
export default {
    props: ["link", "name", "job"]
}
</script>

<style lang="scss" scoped>

.card {
    margin: 20px;
    padding: 20px 0px;
    border-radius: 10px;
    background-color: #56BDF5;
    width: 220px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.profile {
    border-radius: 100px;
    height: 120px;
    width: 120px;
    object-fit: cover;
}

.name {
    margin-top: 20px;
    font-weight: 700;
    font-size: 25px;
}
</style>
