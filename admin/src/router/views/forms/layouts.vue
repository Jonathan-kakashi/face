<script>
import Layout from "../../layouts/main";
import PageHeader from "@/components/page-header";
import appConfig from "@/app.config";

/**
 * Form Layouts component
 */
export default {
  page: {
    title: "Form Layouts",
    meta: [{ name: "description", content: appConfig.description }]
  },
  components: { Layout, PageHeader },
  data() {
    return {
      title: "Form Layouts",
      items: [
        {
          text: "Forms",
          href: "/"
        },
        {
          text: "Form Layouts",
          active: true
        }
      ]
    };
  }
};
</script>

<template>
  <Layout>
    <PageHeader :title="title" :items="items" />
    <div class="row">
      <div class="col-lg-6">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title mb-4">Form grid layout</h4>

            <b-form>
              <b-form-group label="First name" label-for="formrow-firstname-input">
                <b-form-input id="formrow-firstname-input" type="text"></b-form-input>
              </b-form-group>

              <div class="row">
                <div class="col-md-6">
                  <b-form-group label="Email" label-for="formrow-email-input">
                    <b-form-input id="formrow-email-input" type="email"></b-form-input>
                  </b-form-group>
                </div>
                <div class="col-md-6">
                  <div class="form-group">
                    <b-form-group label="Password" label-for="formrow-password-input">
                      <b-form-input id="formrow-password-input" type="email"></b-form-input>
                    </b-form-group>
                  </div>
                </div>
              </div>

              <div class="row">
                <div class="col-lg-4">
                  <b-form-group label="City" label-for="formrow-inputCity">
                    <b-form-input id="formrow-inputCity" type="text"></b-form-input>
                  </b-form-group>
                </div>
                <div class="col-lg-4">
                  <b-form-group id="input-group-1" label="State" label-for="formrow-inputState">
                    <b-form-select
                      id="formrow-inputState"
                      :options="['Choose...', '...']"
                      type="text"
                    ></b-form-select>
                  </b-form-group>
                </div>

                <div class="col-lg-4">
                  <b-form-group label="Zip" label-for="formrow-inputZip">
                    <b-form-input id="formrow-inputZip" type="text"></b-form-input>
                  </b-form-group>
                </div>
              </div>

              <div class="form-group">
                <div class="custom-control custom-checkbox">
                  <input type="checkbox" class="custom-control-input" id="formrow-customCheck" />
                  <label class="custom-control-label" for="formrow-customCheck">Check me out</label>
                </div>
              </div>
              <div>
                <b-button variant="primary">Submit</b-button>
              </div>
            </b-form>
          </div>
        </div>
      </div>

      <div class="col-lg-6">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title mb-4">Horizontal form layout</h4>

            <b-form>
              <b-form-group
                label="First name"
                label-for="horizontal-firstname-input"
                label-cols-sm="3"
              >
                <b-form-input id="horizontal-firstname-input" type="text"></b-form-input>
              </b-form-group>

              <b-form-group
                class="mb-4"
                label="Email"
                label-for="horizontal-email-input"
                label-cols-sm="3"
              >
                <b-form-input id="horizontal-email-input" type="email"></b-form-input>
              </b-form-group>

              <b-form-group
                class="mb-4"
                label="Password"
                label-for="horizontal-password-input"
                label-cols-sm="3"
              >
                <b-form-input id="horizontal-password-input" type="password"></b-form-input>
              </b-form-group>

              <div class="form-group row justify-content-end">
                <div class="col-sm-9">
                  <div class="custom-control custom-checkbox mb-4">
                    <input type="checkbox" class="custom-control-input" id="horizontal-customCheck" />
                    <label class="custom-control-label" for="horizontal-customCheck">Remember me</label>
                  </div>

                  <div>
                    <b-button variant="primary">Submit</b-button>
                  </div>
                </div>
              </div>
            </b-form>
          </div>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-lg-12">
        <div class="card">
          <div class="card-body">
            <h5 class="card-title mb-4">Inline forms layout</h5>

            <b-form inline>
              <label class="sr-only" for="inlineFormInputName2">Name</label>
              <b-input id="inlineFormInputName2" class="mb-2 mr-sm-3" placeholder="Enter Name"></b-input>

              <label class="sr-only" for="inlineFormemail2">Email</label>
              <b-input-group prepend="@" class="mb-2 mr-sm-3">
                <b-input type="email" id="inlineFormemail2" placeholder="Enter Email"></b-input>
              </b-input-group>

              <b-form-checkbox class="mb-2 mr-sm-3">Remember me</b-form-checkbox>

              <b-button variant="primary">Submit</b-button>
            </b-form>
          </div>
        </div>
      </div>
    </div>
    <!--  end row -->
  </Layout>
</template>