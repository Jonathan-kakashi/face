<script>
import appConfig from "@/app.config";

/**
 * Login sample page
 */
export default {
  page: {
    title: "Login",
    meta: [
      {
        name: "description",
        content: appConfig.description,
      },
    ],
  },
};
</script>

<template>
  <div class="account-pages my-5 pt-5">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-md-8 col-lg-6 col-xl-5">
          <div class="card overflow-hidden">
            <div class="bg-soft-primary">
              <div class="row">
                <div class="col-7">
                  <div class="text-primary p-4">
                    <h5 class="text-primary">Welcome Back !</h5>
                    <p>Sign in to continue to Skote.</p>
                  </div>
                </div>
                <div class="col-5 align-self-end">
                  <img
                    src="@/assets/images/profile-img.png"
                    alt
                    class="img-fluid"
                  />
                </div>
              </div>
            </div>
            <div class="card-body pt-0">
              <div>
                <a href="/">
                  <div class="avatar-md profile-user-wid mb-4">
                    <span class="avatar-title rounded-circle bg-light">
                      <img
                        src="@/assets/images/logo.svg"
                        alt
                        class="rounded-circle"
                        height="34"
                      />
                    </span>
                  </div>
                </a>
              </div>
              <div class="p-2">
                <form class="form-horizontal">
                  <div class="form-group">
                    <label for="username">Username</label>
                    <input
                      type="text"
                      class="form-control"
                      id="username"
                      placeholder="Enter username"
                    />
                  </div>

                  <div class="form-group">
                    <label for="userpassword">Password</label>
                    <input
                      type="password"
                      class="form-control"
                      id="userpassword"
                      placeholder="Enter password"
                    />
                  </div>

                  <div class="custom-control custom-checkbox">
                    <input
                      type="checkbox"
                      class="custom-control-input"
                      id="customControlInline"
                    />
                    <label
                      class="custom-control-label"
                      for="customControlInline"
                      >Remember me</label
                    >
                  </div>

                  <div class="mt-3">
                    <button class="btn btn-primary btn-block" type="submit">
                      Log In
                    </button>
                  </div>
                  <div class="mt-4 text-center">
                    <h5 class="font-size-14 mb-3">Sign in with</h5>

                    <ul class="list-inline">
                      <li class="list-inline-item">
                        <a
                          href="javascript: void(0);"
                          class="social-list-item bg-primary text-white border-primary"
                        >
                          <i class="mdi mdi-facebook"></i>
                        </a>
                      </li>
                      <li class="list-inline-item">
                        <a
                          href="javascript: void(0);"
                          class="social-list-item bg-info text-white border-info"
                        >
                          <i class="mdi mdi-twitter"></i>
                        </a>
                      </li>
                      <li class="list-inline-item">
                        <a
                          href="javascript: void(0);"
                          class="social-list-item bg-danger text-white border-danger"
                        >
                          <i class="mdi mdi-google"></i>
                        </a>
                      </li>
                    </ul>
                  </div>

                  <div class="mt-4 text-center">
                    <router-link
                      tag="a"
                      to="/auth/recoverpwd"
                      class="text-muted"
                    >
                      <i class="mdi mdi-lock mr-1"></i> Forgot your password?
                    </router-link>
                  </div>
                </form>
              </div>
            </div>
          </div>
          <div class="mt-5 text-center">
            <p>
              Don't have an account ?
              <router-link
                tag="a"
                to="/auth/register-1"
                class="font-weight-medium text-primary"
                >Signup now</router-link
              >
            </p>
            <p>
              © {{ new Date().getFullYear() }} Skote. Crafted with
              <i class="mdi mdi-heart text-danger"></i> by Themesbrand
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
