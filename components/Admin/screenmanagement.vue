<template>
  <div class="card mb-4">
    <div class="card-header icon-title">
                            <a href="#"><i class="fa fa-shield-alt"></i></a>
                            <h4>Access Control</h4>
                        </div>
    <div class="card-body">
      <nav>
        <ul class="nav sub-tab" id="nav-tab" role="tablist">
          <li class="nav-item">
            <a
              class="nav-link active"
              data-bs-toggle="tab"
              href="#nav-Module"
              role="tab"
              aria-controls="nav-Module"
              aria-selected="true"
              ><i class="fa fas fa-bars"></i> Setting 1: Module</a
            >
          </li>
          <li class="nav-item">
            <a
              class="nav-link"
              id="nav-profile-tab3"
              data-bs-toggle="tab"
              href="#nav-Sub-Module"
              role="tab"
              aria-controls="nav-Sub-Module"
              aria-selected="false"
              ><i class="fa fas fa-align-left"></i> Setting 2: Sub Module</a
            >
          </li>
          <li class="nav-item">
            <a
              class="nav-link"
              id="nav-contact-tab3"
              data-bs-toggle="tab"
              href="#nav-Screen-Page"
              role="tab"
              aria-controls="nav-Screen-Page"
              aria-selected="false"
              ><i class="fa far fa-file"></i> Setting 3: Screen Page</a
            >
          </li>
        
        </ul>
      </nav>

      <div class="tab-content" id="nav-tabContent">
        <div class="tab-pane fade show active" id="nav-Module" role="tabpanel">
          <Module1 />
        </div>

        <div class="tab-pane fade" id="nav-Sub-Module" role="tabpanel">
          <Module2 />
        </div>

        <div class="tab-pane fade" id="nav-Screen-Page" role="tabpanel">
          <Screenpage />
        </div>
       
      </div>
    </div>
  </div>
</template>
<script>
import Module1 from "./Module1.vue";
import Module2 from "./Module2.vue";
import Screenpage from "./screenpage.vue";
export default {
  components: { Module1, Module2, Screenpage},
  name: "screenmanagement",
  setup() {},
};
</script>
