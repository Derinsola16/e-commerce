<template>
  <main class="home">
    <Search />
    <div class="container">
      <Modal />
      <!-- side -->
      <div class="d-flex flex-wrap justify-content-center">
        <!-- image-wrapper  -->
        <!-- <div class="d-flex justify-content-center"> -->
        <div class="mini-card">
          <!-- mini-card@click.prevent="$router.push('/cart')"> -->
          <div class="">
            <!-- inner-wrapper -->
            <div class="p-8 flex-fill">
              <img class="" src="@/assets/image2.png" alt="" />
              <p class="item-name">Wrist Watch for men</p>
              <p class="item-price">$20.58</p>
            </div>
          </div>
        </div>
        <!-- image-wrapper -->
        <div class="mini-card">
          <!-- mini-card -->
          <div class="">
            <!-- inner-wrapper -->
            <div class="p-8 flex-fill">
              <img class="" src="@/assets/image1.png" alt="" />
              <p class="item-name">Heels shoe red in color</p>
              <p class="item-price">$20.58</p>
            </div>
          </div>
        </div>
        <!-- image-wrapper -->
        <div class="mini-card">
          <!-- mini-card -->
          <div class="">
            <!-- inner-wrapper -->
            <div class="p-8 flex-fill">
              <img class="" src="@/assets/image9.png" alt="" />
              <p class="item-name">Gowns</p>
              <p class="item-price">$20.58</p>
            </div>
          </div>
        </div>
        <!-- image-wrapper -->
        <div class="mini-card">
          <!-- mini-card -->
          <div class="">
            <!-- inner-wrapper -->
            <div class="p-8 flex-fill">
              <img class="" src="@/assets/image6.png" alt="" />
              <p class="item-name">Gowns</p>
              <p class="item-price">$20.58</p>
            </div>
          </div>
        </div>
        <!-- image-wrapper -->
        <div class="mini-card">
          <!-- mini-card -->
          <div class="">
            <!-- inner-wrapper -->
            <div class="p-8 flex-fill">
              <img class="" src="@/assets/image7.png" alt="" />
              <p class="item-name">Gowns</p>
              <p class="item-price">$20.58</p>
            </div>
          </div>
        </div>
        <!-- image-wrapper -->
        <div class="mini-card">
          <!-- mini-card -->
          <div class="">
            <!-- inner-wrapper -->
            <div class="p-8 flex-fill">
              <img class="" src="@/assets/image5.png" alt="" />
              <p class="item-name">Short nice Gowns</p>
              <p class="item-price">$20.58</p>
            </div>
          </div>
        </div>
        <!-- </div> -->
      </div>

      <!-- <div>
        I have done deployment but we are having ssl issue and also we only have
        one server for now, that’s the production need to work on the staging
        server that the team can connect to as soon at I solve the ssl issue
      </div> -->
    </div>
  </main>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {
    Search: () => import("@/components/Search.vue"),
    Modal: () => import("@/components/Modal.vue")
  }
};
</script>

<style scoped lang="scss">
.home {
  .mini-card {
    background-color: #ffffff;
    width: 106.3px;
    height: 135px;
    border-radius: 8px;
    margin-bottom: 20px;
    margin-right: 11.7px;
    // padding: 5px;
    box-shadow: 1.5px 3px 15px #e7eaf0 !important;
  }

  .item-name {
    padding-top: 16px;
    font-size: 12px;
    text-align: left;
    color: #3d3d3d;
    line-height: 17px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .item-price {
    font-size: 10px;
    text-align: left;
    width: 31px;
    height: 10px;
    opacity: 100%;
    color: #3d3d3d;
    line-height: 15px;
    font-weight: bold;
  }

  p {
    margin: 0px !important;
  }

  .inner-wrapper {
    min-height: 150px;
    // min-width: 150px;
    margin-left: auto;
    margin-right: auto;
    text-align: center;
    // display: table-cell;
    vertical-align: middle;
  }
}
</style>
