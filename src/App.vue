<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div class="container my-3 my-md-5">
    <div class="row">
      <!-- Sidebar column Start -->
      <div class="col-12 col-md-4 col-lg-4">
        <aside
          class="sidebar text-center px-2 px-md-3 px-lg-5 py-4 py-md-5 rounded"
        >
          <div class="sticky-wrap">
            <div id="user-info" class="user-info">
              <div class="about">
                <img
                  src="assets/images/profile.jpg"
                  class="profile-pic img-fluid rounded-circle"
                />
                <h1 class="name mt-3 mb-1">John Doe</h1>
                <p class="job-name mb-0">Full Stack Developer</p>
              </div>
              <div id="contact-info" class="contact-info mt-5">
                <p class="mb-2">
                  <img src="assets/images/phone.svg" /><a href="#" class="pl-2"
                    >+1-987-719-876</a
                  >
                </p>
                <p class="mb-2">
                  <img src="assets/images/envelope.svg" /><a
                    href="#"
                    class="pl-2"
                    >john@angrystudio.com</a
                  >
                </p>
                <p class="mb-2">
                  <img src="assets/images/link.svg" /><a
                    href="https://angrystudio.com"
                    class="pl-2"
                    >AngryStudio</a
                  >
                </p>
                <div class="social-icons">
                  <ul class="list-unstyled mb-0">
                    <li>
                      <a href="https://github.com">
                        <svg
                          role="img"
                          viewBox="0 0 24 24"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <title>GitHub icon</title>
                          <path
                            d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"
                          />
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href="https://facebook.com">
                        <svg
                          role="img"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 24 24"
                        >
                          <path
                            d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"
                          ></path>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href="https://instagram.com">
                        <svg
                          role="img"
                          viewBox="0 0 24 24"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <path
                            d="M12 0C8.74 0 8.333.015 7.053.072 5.775.132 4.905.333 4.14.63c-.789.306-1.459.717-2.126 1.384S.935 3.35.63 4.14C.333 4.905.131 5.775.072 7.053.012 8.333 0 8.74 0 12s.015 3.667.072 4.947c.06 1.277.261 2.148.558 2.913.306.788.717 1.459 1.384 2.126.667.666 1.336 1.079 2.126 1.384.766.296 1.636.499 2.913.558C8.333 23.988 8.74 24 12 24s3.667-.015 4.947-.072c1.277-.06 2.148-.262 2.913-.558.788-.306 1.459-.718 2.126-1.384.666-.667 1.079-1.335 1.384-2.126.296-.765.499-1.636.558-2.913.06-1.28.072-1.687.072-4.947s-.015-3.667-.072-4.947c-.06-1.277-.262-2.149-.558-2.913-.306-.789-.718-1.459-1.384-2.126C21.319 1.347 20.651.935 19.86.63c-.765-.297-1.636-.499-2.913-.558C15.667.012 15.26 0 12 0zm0 2.16c3.203 0 3.585.016 4.85.071 1.17.055 1.805.249 2.227.415.562.217.96.477 1.382.896.419.42.679.819.896 1.381.164.422.36 1.057.413 2.227.057 1.266.07 1.646.07 4.85s-.015 3.585-.074 4.85c-.061 1.17-.256 1.805-.421 2.227-.224.562-.479.96-.899 1.382-.419.419-.824.679-1.38.896-.42.164-1.065.36-2.235.413-1.274.057-1.649.07-4.859.07-3.211 0-3.586-.015-4.859-.074-1.171-.061-1.816-.256-2.236-.421-.569-.224-.96-.479-1.379-.899-.421-.419-.69-.824-.9-1.38-.165-.42-.359-1.065-.42-2.235-.045-1.26-.061-1.649-.061-4.844 0-3.196.016-3.586.061-4.861.061-1.17.255-1.814.42-2.234.21-.57.479-.96.9-1.381.419-.419.81-.689 1.379-.898.42-.166 1.051-.361 2.221-.421 1.275-.045 1.65-.06 4.859-.06l.045.03zm0 3.678c-3.405 0-6.162 2.76-6.162 6.162 0 3.405 2.76 6.162 6.162 6.162 3.405 0 6.162-2.76 6.162-6.162 0-3.405-2.76-6.162-6.162-6.162zM12 16c-2.21 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm7.846-10.405c0 .795-.646 1.44-1.44 1.44-.795 0-1.44-.646-1.44-1.44 0-.794.646-1.439 1.44-1.439.793-.001 1.44.645 1.44 1.439z"
                          ></path>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href="https://linkedin.com">
                        <svg
                          role="img"
                          viewBox="0 0 24 24"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <path
                            d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"
                          ></path>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href="https://pinterest.com">
                        <svg
                          role="img"
                          viewBox="0 0 24 24"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <path
                            d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 5.079 3.158 9.417 7.618 11.162-.105-.949-.199-2.403.041-3.439.219-.937 1.406-5.957 1.406-5.957s-.359-.72-.359-1.781c0-1.663.967-2.911 2.168-2.911 1.024 0 1.518.769 1.518 1.688 0 1.029-.653 2.567-.992 3.992-.285 1.193.6 2.165 1.775 2.165 2.128 0 3.768-2.245 3.768-5.487 0-2.861-2.063-4.869-5.008-4.869-3.41 0-5.409 2.562-5.409 5.199 0 1.033.394 2.143.889 2.741.099.12.112.225.085.345-.09.375-.293 1.199-.334 1.363-.053.225-.172.271-.401.165-1.495-.69-2.433-2.878-2.433-4.646 0-3.776 2.748-7.252 7.92-7.252 4.158 0 7.392 2.967 7.392 6.923 0 4.135-2.607 7.462-6.233 7.462-1.214 0-2.354-.629-2.758-1.379l-.749 2.848c-.269 1.045-1.004 2.352-1.498 3.146 1.123.345 2.306.535 3.55.535 6.607 0 11.985-5.365 11.985-11.987C23.97 5.39 18.592.026 11.985.026L12.017 0z"
                          ></path>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href="https://twitter.com">
                        <svg
                          role="img"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 24 24"
                        >
                          <path
                            d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"
                          ></path>
                        </svg>
                      </a>
                    </li>
                    <li>
                      <a href="https://youtube.com">
                        <svg
                          role="img"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 24 24"
                        >
                          &gt;
                          <path
                            d="M23.499 6.203a3.008 3.008 0 00-2.089-2.089c-1.87-.501-9.4-.501-9.4-.501s-7.509-.01-9.399.501a3.008 3.008 0 00-2.088 2.09A31.258 31.26 0 000 12.01a31.258 31.26 0 00.523 5.785 3.008 3.008 0 002.088 2.089c1.869.502 9.4.502 9.4.502s7.508 0 9.399-.502a3.008 3.008 0 002.089-2.09 31.258 31.26 0 00.5-5.784 31.258 31.26 0 00-.5-5.808zm-13.891 9.4V8.407l6.266 3.604z"
                          ></path>
                        </svg>
                      </a>
                    </li>
                  </ul>
                </div>
                <div class="contact-btn">
                  <a
                    href="#"
                    class="btn btn-primary btn-sm mt-5 rounded-pill text-uppercase"
                    onclick="showForm(event)"
                    >Contact</a
                  >
                </div>
              </div>
            </div>
            <div id="contact-form" class="contact-form mt-4">
              <div class="row align-items-center">
                <div class="col-6 text-left">
                  <h3 class="form-title text-uppercase pl-3 mb-0">Say Hi!</h3>
                </div>
                <div class="col-6 text-right">
                  <button
                    id="close-form"
                    class="close-form bg-transparent border-0 pr-3"
                    onclick="showUserInfo(event)"
                  >
                    <svg
                      version="1.1"
                      id="Capa_1"
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:xlink="http://www.w3.org/1999/xlink"
                      x="0px"
                      y="0px"
                      viewBox="0 0 490 490"
                      style="enable-background: new 0 0 490 490"
                      xml:space="preserve"
                    >
                      <polygon
                        points="456.851,0 245,212.564 33.149,0 0.708,32.337 212.669,245.004 0.708,457.678 33.149,490 245,277.443 456.851,490 
										489.292,457.678 277.331,245.004 489.292,32.337 "
                      />
                    </svg>
                  </button>
                </div>
              </div>
              <form action="#" method="POST" class="mt-1">
                <input
                  type="text"
                  class="form-control bg-transparent rounded-pill mb-3"
                  placeholder="Name"
                />
                <input
                  type="text"
                  class="form-control bg-transparent rounded-pill mb-3"
                  placeholder="Email"
                />
                <textarea
                  class="form-control bg-transparent rounded-pill mb-3"
                  placeholder="Message"
                ></textarea>
                <button
                  type="button"
                  class="btn btn-primary btn-sm text-uppercase rounded-pill"
                >
                  Submit
                </button>
              </form>
            </div>
          </div>
        </aside>
      </div>
      <!-- Sidebar column End -->
      <!-- Main Content column Start -->
      <div class="col-12 col-md-8 col-lg-8">
        <main class="content ml-0 ml-md-2 mr-0">
          <!-- About  Start-->
          <div id="about" class="section mt-3 mt-md-0 p-3 p-md-5 rounded">
            <h3 class="mb-3 text-uppercase">About</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
              accumsan turpis nec elit feugiat, et sodales ex pulvinar. Donec
              dolor massa, consequat eu interdum a, semper at lectus. Aliquam
              risus nibh, placerat eget condimentum id, eleifend quis tortor.
              Phasellus vel lacus urna. Nulla facilisi. Duis a purus vitae elit
              finibus aliquam. Aenean ut lectus quis ex eleifend imperdiet. In
              vitae mattis nibh. Vivamus nec lectus ac justo iaculis interdum.
            </p>
          </div>
          <!-- About  End-->
          <!-- Education  Start-->
          <div id="education" class="section mt-3 mt-md-5 p-3 p-md-5 rounded">
            <h3 class="mb-2 text-uppercase">Education</h3>
            <div class="row mt-4 mb-2">
              <div class="col-6">
                <span class="tiny-super font-weight-bold"
                  >Master Of Engineering</span
                >
                <span class="tiny-super d-block">MIT</span>
              </div>
              <div class="col-6 text-right">
                <span class="tiny-super">2010 - 2012</span>
              </div>
            </div>
            <div class="row mt-4 mb-2">
              <div class="col-6">
                <span class="tiny-super font-weight-bold"
                  >Bachelor Of Engineering</span
                >
                <span class="tiny-super d-block">KIP</span>
              </div>
              <div class="col-6 text-right">
                <span class="tiny-super">2007 - 2010</span>
              </div>
            </div>
          </div>
          <!-- Education  End-->
          <!-- Experience  Start-->
          <div id="experience" class="section mt-3 mt-md-5 p-3 p-md-5 rounded">
            <h3 class="mb-3 text-uppercase">Work Experience</h3>
            <div class="row mt-4 mb-2">
              <div class="col-6">
                <span class="tiny-super font-weight-bold"
                  >Full Stack Developer</span
                >
                <span class="tiny-super d-block">Amazon</span>
              </div>
              <div class="col-6 text-right">
                <span class="tiny-super">2017 - Present</span>
              </div>
              <div class="col-12 mt-2">
                <p>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
                  accumsan turpis nec elit feugiat, et sodales ex pulvinar.
                  Donec dolor massa, consequat eu interdum a, semper at lectus.
                  Aliquam risus nibh, placerat eget condimentum id, eleifend
                  quis tortor. Phasellus vel lacus urna. Nulla facilisi. Duis a
                  purus vitae elit finibus aliquam.
                </p>
              </div>
            </div>
            <div class="row mt-4 mb-2">
              <div class="col-6">
                <span class="tiny-super font-weight-bold">Web Developer</span>
                <span class="tiny-super d-block">Google</span>
              </div>
              <div class="col-6 text-right">
                <span class="tiny-super">2015 - 2017</span>
              </div>
              <div class="col-12 mt-2">
                <p>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
                  accumsan turpis nec elit feugiat, et sodales ex pulvinar.
                  Donec dolor massa, consequat eu interdum a, semper at lectus.
                  Aliquam risus nibh, placerat eget condimentum id, eleifend
                  quis tortor. Phasellus vel lacus urna. Nulla facilisi. Duis a
                  purus vitae elit finibus aliquam.
                </p>
              </div>
            </div>
            <div class="row mt-4 mb-2">
              <div class="col-6">
                <span class="tiny-super font-weight-bold"
                  >Web Developer Intern</span
                >
                <span class="tiny-super d-block">MIT</span>
              </div>
              <div class="col-6 text-right">
                <span class="tiny-super">2015 - 2017</span>
              </div>
              <div class="col-12 mt-2">
                <p>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
                  accumsan turpis nec elit feugiat, et sodales ex pulvinar.
                  Donec dolor massa, consequat eu interdum a, semper at lectus.
                  Aliquam risus nibh, placerat eget condimentum id, eleifend
                  quis tortor. Phasellus vel lacus urna. Nulla facilisi. Duis a
                  purus vitae elit finibus aliquam.
                </p>
              </div>
            </div>
          </div>
          <!-- Experience End-->
          <!-- Projects  Start-->
          <div id="projects" class="section mt-3 mt-md-5 p-3 p-md-5 rounded">
            <h3 class="mb-3 text-uppercase">Projects</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
              accumsan turpis nec elit feugiat, et sodales ex pulvinar. Donec
              dolor massa, consequat eu interdum a, semper at lectus.
            </p>
            <p>
              <strong>Apps - </strong>Ut accumsan turpis nec elit feugiat, et
              sodales ex pulvinar. Donec dolor massa, consequat eu interdum a,
              semper at lectus.
            </p>
            <p>
              <strong>CRMs - </strong>Ut accumsan turpis nec elit feugiat, et
              sodales ex pulvinar. Donec dolor massa, consequat eu interdum a,
              semper at lectus.
            </p>
            <p>
              <strong>Websites - </strong>Ut accumsan turpis nec elit feugiat,
              et sodales ex pulvinar. Donec dolor massa, consequat eu interdum
              a, semper at lectus.
            </p>
            <p>
              <strong>eCom Apps - </strong>Ut accumsan turpis nec elit feugiat,
              et sodales ex pulvinar. Donec dolor massa, consequat eu interdum
              a, semper at lectus.
            </p>
          </div>
          <!-- Projects  End-->
          <!-- Certifications  Start-->
          <div
            id="certifications"
            class="section mt-3 mt-md-5 p-3 p-md-5 rounded"
          >
            <h3 class="mb-3 text-uppercase">Certifications</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
              accumsan turpis nec elit feugiat, et sodales ex pulvinar. Donec
              dolor massa, consequat eu interdum a, semper at lectus.
            </p>
            <p>
              <strong>SAP - </strong>Ut accumsan turpis nec elit feugiat, et
              sodales ex pulvinar. Donec dolor massa, consequat eu interdum a,
              semper at lectus.
            </p>
            <p>
              <strong>CCP - </strong>Ut accumsan turpis nec elit feugiat, et
              sodales ex pulvinar. Donec dolor massa, consequat eu interdum a,
              semper at lectus.
            </p>
            <p>
              <strong>PAAS - </strong>Ut accumsan turpis nec elit feugiat, et
              sodales ex pulvinar. Donec dolor massa, consequat eu interdum a,
              semper at lectus.
            </p>
            <p>
              <strong>HDPCD - </strong>Ut accumsan turpis nec elit feugiat, et
              sodales ex pulvinar. Donec dolor massa, consequat eu interdum a,
              semper at lectus.
            </p>
          </div>
          <!-- Certifications  End-->
          <!-- Skills  Start-->
          <div id="skills" class="section mt-3 mt-md-5 p-3 p-md-5 rounded">
            <h3 class="mb-3 text-uppercase">Skills</h3>
            <div class="row">
              <div class="col-12">
                <p>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut
                  accumsan turpis nec elit feugiat, et sodales ex pulvinar.
                  Donec dolor massa, consequat eu interdum
                </p>
              </div>
              <div class="col-12 col-md-6">
                <div class="progress mt-4">
                  <div
                    class="progress-bar progress-bar-striped progress-bar-animated bg-progress"
                    role="progressbar"
                    aria-valuenow="95"
                    aria-valuemin="0"
                    aria-valuemax="100"
                    style="width: 95%"
                  >
                    Python
                  </div>
                </div>
                <div class="progress mt-4">
                  <div
                    class="progress-bar progress-bar-striped progress-bar-animated bg-progress"
                    role="progressbar"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                    style="width: 90%"
                  >
                    JavaScript
                  </div>
                </div>
                <div class="progress mt-4">
                  <div
                    class="progress-bar progress-bar-striped progress-bar-animated bg-progress"
                    role="progressbar"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                    style="width: 90%"
                  >
                    Go
                  </div>
                </div>
              </div>
              <div class="col-12 col-md-6">
                <div class="progress mt-4">
                  <div
                    class="progress-bar progress-bar-striped progress-bar-animated bg-progress"
                    role="progressbar"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                    style="width: 90%"
                  >
                    PHP
                  </div>
                </div>
                <div class="progress mt-4">
                  <div
                    class="progress-bar progress-bar-striped progress-bar-animated bg-progress"
                    role="progressbar"
                    aria-valuenow="85"
                    aria-valuemin="0"
                    aria-valuemax="100"
                    style="width: 85%"
                  >
                    JAVA
                  </div>
                </div>
                <div class="progress mt-4">
                  <div
                    class="progress-bar progress-bar-striped progress-bar-animated bg-progress"
                    role="progressbar"
                    aria-valuenow="80"
                    aria-valuemin="0"
                    aria-valuemax="100"
                    style="width: 90%"
                  >
                    Pearl
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Skills  End-->
        </main>
      </div>
      <!-- Main Content column End -->
    </div>
  </div>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
