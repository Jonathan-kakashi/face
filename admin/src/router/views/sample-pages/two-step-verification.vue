<script>
import appConfig from "@/app.config";

/**
 * Two-step-verification component
 */
export default {
  page: {
    title: "Two step verification",
    meta: [{ name: "description", content: appConfig.description }],
  },
  data() {
    return {};
  },
  components: {},
  methods: {},
};
</script>

<template>
  <div class="account-pages my-5 pt-sm-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="text-center mb-5 text-muted">
            <router-link to="/" class="d-block auth-logo">
              <img
                src="@/assets/images/logo-dark.png"
                alt=""
                height="20"
                class="auth-logo-dark mx-auto"
              />
              <img
                src="@/assets/images/logo-light.png"
                alt=""
                height="20"
                class="auth-logo-light mx-auto"
              />
            </router-link>
            <p class="mt-3">Responsive Bootstrap 4 Admin Dashboard</p>
          </div>
        </div>
      </div>
      <!-- end row -->
      <div class="row justify-content-center">
        <div class="col-md-8 col-lg-6 col-xl-5">
          <div class="card">
            <div class="card-body">
              <div class="p-2">
                <div class="text-center">
                  <div class="avatar-md mx-auto">
                    <div class="avatar-title rounded-circle bg-light">
                      <i class="bx bxs-envelope h1 mb-0 text-primary"></i>
                    </div>
                  </div>
                  <div class="p-2 mt-4">
                    <h4>Verify your email</h4>
                    <p class="mb-5">
                      Please enter the 4 digit code sent to
                      <span class="font-weight-semibold">example@abc.com</span>
                    </p>

                    <form>
                      <div class="row">
                        <div class="col-3">
                          <div class="form-group">
                            <label for="digit1-input" class="sr-only"
                              >Dight 1</label
                            >
                            <input
                              type="text"
                              class="form-control form-control-lg text-center"
                              onkeyup="moveToNext(this, 2)"
                              maxLength="1"
                              id="digit1-input"
                            />
                          </div>
                        </div>

                        <div class="col-3">
                          <div class="form-group">
                            <label for="digit2-input" class="sr-only"
                              >Dight 2</label
                            >
                            <input
                              type="text"
                              class="form-control form-control-lg text-center"
                              onkeyup="moveToNext(this, 3)"
                              maxLength="1"
                              id="digit2-input"
                            />
                          </div>
                        </div>

                        <div class="col-3">
                          <div class="form-group">
                            <label for="digit3-input" class="sr-only"
                              >Dight 3</label
                            >
                            <input
                              type="text"
                              class="form-control form-control-lg text-center"
                              onkeyup="moveToNext(this, 4)"
                              maxLength="1"
                              id="digit3-input"
                            />
                          </div>
                        </div>

                        <div class="col-3">
                          <div class="form-group">
                            <label for="digit4-input" class="sr-only"
                              >Dight 4</label
                            >
                            <input
                              type="text"
                              class="form-control form-control-lg text-center"
                              onkeyup="moveToNext(this, 4)"
                              maxLength="1"
                              id="digit4-input"
                            />
                          </div>
                        </div>
                      </div>
                    </form>

                    <div class="mt-4">
                      <router-link to="/" class="btn btn-success w-md"
                        >Confirm</router-link
                      >
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="mt-5 text-center">
            <p>
              Did't receive a code ?
              <a href="#" class="font-weight-medium text-primary"> Resend </a>
            </p>
            <p>
              ©
              {{ new Date().getFullYear() }}
              Skote. Crafted with <i class="mdi mdi-heart text-danger"></i> by
              Themesbrand
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>