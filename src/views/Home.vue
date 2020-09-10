<template>
  <div>
    <AppNavbar></AppNavbar>

    <h3 style="padding-left: 4rem">Characters</h3>

    <div class="container">
      <div class="row">
        <div class="col-sm-3 mb-3" v-for="item in 8" :key="item">
          <div class="card w-75">
            <img
              src="@/assets/logo.png"
              width="150"
              height="150"
              class="card-img-bottom"
              alt="character"
            />
            <div class="card-footer bg-dark">Card {{ item }}</div>
          </div>
        </div>
      </div>
    </div>

    <AppFooter></AppFooter>
  </div>
</template>

<script>
// @ is an alias to /src
import AppNavbar from '@/components/AppNavbar'
import AppFooter from '@/components/AppFooter'

export default {
  name: 'Home',
  components: {
    AppNavbar,
    AppFooter
  }
}
</script>

<style scoped></style>
