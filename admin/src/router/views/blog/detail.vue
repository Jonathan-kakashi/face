<script>
import Layout from "../../layouts/main";
import PageHeader from "@/components/page-header";
import appConfig from "@/app.config";

export default {
  page: {
    title: "Blog Detail",
    meta: [{ name: "description", content: appConfig.description }],
  },
  components: {
    Layout,
    PageHeader,
  },
  data() {
    return {
      title: "Blog Detail",
      items: [
        {
          text: "Blog",
          href: "/",
        },
        {
          text: "Blog Detail",
          active: true,
        },
      ],
    };
  },
};
</script>

<template>
  <Layout>
    <PageHeader :title="title" :items="items" />
    <div class="row">
      <div class="col-lg-12">
        <div class="card">
          <div class="card-body">
            <div class="pt-3">
              <div class="row justify-content-center">
                <div class="col-xl-8">
                  <div>
                    <div class="text-center">
                      <div class="mb-4">
                        <a href="#" class="badge badge-light font-size-12">
                          <i
                            class="bx bx-purchase-tag-alt align-middle text-muted mr-1"
                          ></i>
                          Project
                        </a>
                      </div>
                      <h4>Beautiful Day with Friends</h4>
                      <p class="text-muted mb-4">
                        <i class="mdi mdi-calendar mr-1"></i> 10 Apr, 2020
                      </p>
                    </div>

                    <hr />
                    <div class="text-center">
                      <div class="row">
                        <div class="col-sm-4">
                          <div>
                            <p class="text-muted mb-2">Categories</p>
                            <h5 class="font-size-15">Project</h5>
                          </div>
                        </div>
                        <div class="col-sm-4">
                          <div class="mt-4 mt-sm-0">
                            <p class="text-muted mb-2">Date</p>
                            <h5 class="font-size-15">10 Apr, 2020</h5>
                          </div>
                        </div>
                        <div class="col-sm-4">
                          <div class="mt-4 mt-sm-0">
                            <p class="text-muted mb-2">Post by</p>
                            <h5 class="font-size-15">Gilbert Smith</h5>
                          </div>
                        </div>
                      </div>
                    </div>
                    <hr />

                    <div class="my-5">
                      <img
                        src="@/assets/images/small/img-2.jpg"
                        alt=""
                        class="img-thumbnail mx-auto d-block"
                      />
                    </div>

                    <hr />

                    <div class="mt-4">
                      <div class="text-muted font-size-14">
                        <p>
                          Neque porro quisquam est, qui dolorem ipsum quia dolor
                          sit amet, consectetur, adipisci velit, sed quia non
                          numquam eius modi tempora incidunt ut labore et dolore
                          magnam enim ad minima veniam quis
                        </p>

                        <p class="mb-4">
                          Ut enim ad minima veniam, quis nostrum exercitationem
                          ullam corporis suscipit laboriosam, nisi ut aliquid ex
                          ea reprehenderit qui in ea voluptate velit esse quam
                          nihil molestiae consequatur, vel illum qui dolorem eum
                          fugiat quo voluptas nulla pariatur? At vero eos et
                          accusamus et iusto odio dignissimos ducimus qui
                          blanditiis praesentium voluptatum deleniti atque
                          corrupti quos dolores et quas molestias excepturi sint
                          occaecati cupiditate non provident, similique sunt
                        </p>

                        <blockquote
                          class="p-4 border-light border rounded mb-4"
                        >
                          <div class="d-flex">
                            <div class="mr-3">
                              <i
                                class="bx bxs-quote-alt-left text-dark font-size-24"
                              ></i>
                            </div>
                            <div>
                              <p class="mb-0">
                                At vero eos et accusamus et iusto odio
                                dignissimos ducimus qui blanditiis praesentium
                                deleniti atque corrupti quos dolores et quas
                                molestias excepturi sint quidem rerum facilis
                                est
                              </p>
                            </div>
                          </div>
                        </blockquote>

                        <p>
                          Itaque earum rerum hic tenetur a sapiente delectus, ut
                          aut reiciendis voluptatibus maiores alias consequatur
                          aut perferendis doloribus asperiores repellat. Sed ut
                          perspiciatis unde omnis iste natus error sit
                        </p>

                        <div class="mt-4">
                          <h5 class="mb-3">Title:</h5>

                          <div>
                            <div class="row">
                              <div class="col-lg-4 col-sm-6">
                                <div>
                                  <ul class="pl-4">
                                    <li class="py-1">Donec sodales sagittis</li>
                                    <li class="py-1">Sed consequat leo eget</li>
                                    <li class="py-1">Aliquam lorem ante</li>
                                  </ul>
                                </div>
                              </div>
                              <div class="col-lg-4 col-sm-6">
                                <div>
                                  <ul class="pl-4">
                                    <li class="py-1">Aenean ligula eget</li>
                                    <li class="py-1">Cum sociis natoque</li>
                                  </ul>
                                </div>
                              </div>
                            </div>
                          </div>
                        </div>
                      </div>

                      <hr />

                      <div class="mt-5">
                        <h5 class="font-size-15">
                          <i
                            class="bx bx-message-dots text-muted align-middle mr-1"
                          ></i>
                          Comments :
                        </h5>

                        <div>
                          <div class="media py-3">
                            <div class="avatar-xs mr-3">
                              <div
                                class="avatar-title rounded-circle bg-light text-primary"
                              >
                                <i class="bx bxs-user"></i>
                              </div>
                            </div>
                            <div class="media-body">
                              <h5 class="font-size-14 mb-1">
                                Delores Williams
                                <small class="text-muted float-right"
                                  >1 hr Ago</small
                                >
                              </h5>
                              <p class="text-muted">
                                If several languages coalesce, the grammar of
                                the resulting language is more simple and
                                regular than that of the individual
                              </p>
                              <div>
                                <a
                                  href="javascript: void(0);"
                                  class="text-success"
                                  ><i class="mdi mdi-reply"></i> Reply</a
                                >
                              </div>
                            </div>
                          </div>
                          <div class="media py-3 border-top">
                            <div class="avatar-xs mr-3">
                              <img
                                src="@/assets/images/users/avatar-2.jpg"
                                alt=""
                                class="img-fluid d-block rounded-circle"
                              />
                            </div>
                            <div class="media-body">
                              <h5 class="font-size-14 mb-1">
                                Clarence Smith
                                <small class="text-muted float-right"
                                  >2 hrs Ago</small
                                >
                              </h5>
                              <p class="text-muted">
                                Neque porro quisquam est, qui dolorem ipsum quia
                                dolor sit amet
                              </p>
                              <div>
                                <a
                                  href="javascript: void(0);"
                                  class="text-success"
                                  ><i class="mdi mdi-reply"></i> Reply</a
                                >
                              </div>

                              <div class="media pt-3">
                                <div class="avatar-xs mr-3">
                                  <div
                                    class="avatar-title rounded-circle bg-light text-primary"
                                  >
                                    <i class="bx bxs-user"></i>
                                  </div>
                                </div>
                                <div class="media-body">
                                  <h5 class="font-size-14 mb-1">
                                    Silvia Martinez
                                    <small class="text-muted float-right"
                                      >2 hrs Ago</small
                                    >
                                  </h5>
                                  <p class="text-muted">
                                    To take a trivial example, which of us ever
                                    undertakes laborious physical exercise
                                  </p>
                                  <div>
                                    <a
                                      href="javascript: void(0);"
                                      class="text-success"
                                      ><i class="mdi mdi-reply"></i> Reply</a
                                    >
                                  </div>
                                </div>
                              </div>
                            </div>
                          </div>

                          <div class="media py-3 border-top">
                            <div class="avatar-xs mr-3">
                              <div
                                class="avatar-title rounded-circle bg-light text-primary"
                              >
                                <i class="bx bxs-user"></i>
                              </div>
                            </div>
                            <div class="media-body">
                              <h5 class="font-size-14 mb-1">
                                Keith McCoy
                                <small class="text-muted float-right"
                                  >12 Aug</small
                                >
                              </h5>
                              <p class="text-muted">
                                Donec posuere vulputate arcu. phasellus accumsan
                                cursus velit
                              </p>
                              <div>
                                <a
                                  href="javascript: void(0);"
                                  class="text-success"
                                  ><i class="mdi mdi-reply"></i> Reply</a
                                >
                              </div>
                            </div>
                          </div>
                        </div>
                      </div>

                      <div class="mt-4">
                        <h5 class="font-size-16 mb-3">Leave a Message</h5>

                        <form>
                          <div class="row">
                            <div class="col-md-6">
                              <div class="form-group">
                                <label for="commentname-input">Name</label>
                                <input
                                  type="text"
                                  class="form-control"
                                  id="commentname-input"
                                  placeholder="Enter name"
                                />
                              </div>
                            </div>
                            <div class="col-md-6">
                              <div class="form-group">
                                <label for="commentemail-input">Email</label>
                                <input
                                  type="email"
                                  class="form-control"
                                  id="commentemail-input"
                                  placeholder="Enter email"
                                />
                              </div>
                            </div>
                          </div>

                          <div class="form-group">
                            <label for="commentmessage-input">Message</label>
                            <textarea
                              class="form-control"
                              id="commentmessage-input"
                              placeholder="Your message..."
                              rows="3"
                            ></textarea>
                          </div>

                          <div class="text-right">
                            <button type="submit" class="btn btn-success w-sm">
                              Submit
                            </button>
                          </div>
                        </form>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- end card body -->
        </div>
        <!-- end card -->
      </div>
      <!-- end col -->
    </div>
    <!-- end row -->
  </Layout>
</template>