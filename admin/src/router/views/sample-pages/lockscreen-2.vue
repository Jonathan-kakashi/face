<script>
import { Carousel, Slide } from "vue-carousel";
import appConfig from "@/app.config";

/**
 * Lockscreen-2 component
 */
export default {
  page: {
    title: "Lockscreen 2",
    meta: [{ name: "description", content: appConfig.description }],
  },
  data() {
    return {};
  },
  components: {
    Carousel,
    Slide,
  },
  methods: {
    nextSlide() {
      this.$refs.carousel.goToPage(this.$refs.carousel.getNextPage());
    },
    prevSlide() {
      this.$refs.carousel.goToPage(this.$refs.carousel.getPreviousPage());
    },
  },
  mounted() {
    document.body.classList.add("auth-body-bg");
  },
};
</script>

<template>
  <div>
    <div class="container-fluid p-0">
      <div class="row no-gutters">
        <div class="col-xl-9">
          <div class="auth-full-bg pt-lg-5 p-4">
            <div class="w-100">
              <div class="bg-overlay"></div>
              <div class="d-flex h-100 flex-column">
                <div class="p-4 mt-auto">
                  <div class="row justify-content-center">
                    <div class="col-lg-7">
                      <div class="text-center">
                        <h4 class="mb-3">
                          <i
                            class="bx bxs-quote-alt-left text-primary h1 align-middle mr-3"
                          ></i
                          ><span class="text-primary">5k</span>+ Satisfied
                          clients
                        </h4>

                        <div dir="ltr">
                          <carousel
                            ref="carousel"
                            class="navs-carousel auth-review-carousel owl-theme"
                            id="timeline-carousel"
                            :navigation-enabled="false"
                            :pagination-active-color="'#556ee6'"
                            :pagination-color="'#556ee640'"
                            :pagination-position="'2'"
                            :pagination-padding="8"
                            :perPageCustom="[
                              [480, 1],
                              [768, 1],
                            ]"
                          >
                            <slide>
                              <div class="item">
                                <div class="py-3">
                                  <p class="font-size-16 mb-4">
                                    " Fantastic theme with a ton of options. If
                                    you just want the HTML to integrate with
                                    your project, then this is the package. You
                                    can find the files in the 'dist' folder...no
                                    need to install git and all the other stuff
                                    the documentation talks about. "
                                  </p>

                                  <div>
                                    <h4 class="font-size-16 text-primary">
                                      Abs1981
                                    </h4>
                                    <p class="font-size-14 mb-0">
                                      - Skote User
                                    </p>
                                  </div>
                                </div>
                              </div>
                            </slide>
                            <slide>
                              <div class="item">
                                <div class="py-3">
                                  <p class="font-size-16 mb-4">
                                    " If Every Vendor on Envato are as
                                    supportive as Themesbrand, Development with
                                    be a nice experience. You guys are
                                    Wonderful. Keep us the good work. "
                                  </p>

                                  <div>
                                    <h4 class="font-size-16 text-primary">
                                      nezerious
                                    </h4>
                                    <p class="font-size-14 mb-0">
                                      - Skote User
                                    </p>
                                  </div>
                                </div>
                              </div>
                            </slide>
                          </carousel>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- end col -->

        <div class="col-xl-3">
          <div class="auth-full-page-content p-md-5 p-4">
            <div class="w-100">
              <div class="d-flex flex-column h-100">
                <div class="mb-4 mb-md-5">
                  <router-link to="/" class="d-block auth-logo">
                    <img
                      src="@/assets/images/logo-dark.png"
                      alt=""
                      height="18"
                      class="auth-logo-dark"
                    />
                    <img
                      src="@/assets/images/logo-light.png"
                      alt=""
                      height="18"
                      class="auth-logo-light"
                    />
                  </router-link>
                </div>
                <div class="my-auto">
                  <div>
                    <h5 class="text-primary">Lock screen</h5>
                    <p class="text-muted">
                      Enter your password to unlock the screen!
                    </p>
                  </div>

                  <div class="mt-4">
                    <form class="form-horizontal">
                      <div class="user-thumb text-center mb-4">
                        <img
                          src="@/assets/images/users/avatar-1.jpg"
                          class="rounded-circle img-thumbnail avatar-md"
                          alt="thumbnail"
                        />
                        <h5 class="font-size-15 mt-3">Maria Laird</h5>
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

                      <div class="form-group row mb-0">
                        <div class="col-12 text-right">
                          <button
                            class="btn btn-primary w-md waves-effect waves-light"
                            type="submit"
                          >
                            Unlock
                          </button>
                        </div>
                      </div>
                    </form>
                    <div class="mt-5 text-center">
                      <p>
                        Not you ? return
                        <router-link
                          to="/auth/login-2"
                          class="font-weight-medium text-primary"
                        >
                          Sign In
                        </router-link>
                      </p>
                    </div>
                  </div>
                </div>

                <div class="mt-4 mt-md-5 text-center">
                  <p class="mb-0">
                    © {{ new Date().getFullYear() }} Skote. Crafted with
                    <i class="mdi mdi-heart text-danger"></i> by Themesbrand
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- end col -->
      </div>
      <!-- end row -->
    </div>
    <!-- end container-fluid -->
  </div>
</template>