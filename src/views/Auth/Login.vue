<template>
  <main class="sign-up">
    <header class="d-flex justify-content-start p-16">
      <a href="" @click.prevent="$router.go(-1)" class="text-grey-800">
        <i class="fas fa-arrow-left"></i>
      </a>
    </header>

    <div class="body container d-flex flex-wrap justify-content-center">
      <!-- Logo will be here -->
      <div class="content">
        <div class="text-primary flex-wrap">
          <div class="heading text-grey-100">SIGN IN</div>
          <p class="content-text mb-32 pl-32 pr-32">
            By creating an account, you agree to our Terms of Service and
            Privacy Policy
          </p>
        </div>
        <div class="">
          <form>
            <div class="wrapper">
              <i class="far fa-envelope icon"></i>
              <input
                id="input-1"
                class="form-control mb-24"
                type="email"
                required
                placeholder="Enter email"
              />
            </div>
            <div class="wrapper">
              <i class="fas fa-lock icon"></i>
              <input
                id="input-1"
                class="form-control mb-48"
                type="password"
                required
                placeholder="Enter Password"
              />
            </div>

            <div>
              <button
                class="btn btn-secondary mb-16"
                type="button"
                @click.prevent="register"
              >
                SIGN IN
              </button>
            </div>
          </form>
          <p class="text-primary">Don't have an account?</p>
          <router-link to="/sign-up" class="text-secondary">
            Create a new one
          </router-link>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  methods: {
    async register() {
      this.$router.push("/");
    }
  }
};
</script>

<style lang="scss" scoped>
.sign-up {
  width: 100%;
  height: auto;

  .body {
    padding: 5rem 0rem 2.28rem;
    text-align: center;

    .content {
      padding-top: 30px;

      .heading {
        font-size: 32px;
        font-weight: bold;
      }

      .content-text {
        width: 260px;
        text-align: center;
        margin: auto;
        padding: 15px;
      }

      .bottom-text {
        position: relative;
        top: 5vh;
        color: #b3b3b3;

        a {
          text-decoration: none;
          color: #096dd9;
          display: none;
        }
      }
    }
  }

  .form-control {
    width: 100%;
    height: 50px;
    box-sizing: border-box;
    border: 1px solid #707070;
    border-radius: 10px;
    font-size: 16px;
    background-color: white;
    background-position: 10px 10px;
    background-repeat: no-repeat;
    padding-left: 43px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    color: #000;
    // transition: width 0.4s ease-in-out;
  }

  .wrapper {
    position: relative;
  }

  .icon {
    position: absolute;
    left: 15px;
    top: 17px;
    color: #484848;
  }
}
</style>
