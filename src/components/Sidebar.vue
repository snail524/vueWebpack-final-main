<template>
    <div>
    <nav id="sidebarMenu" class="col-md-3 col-lg-2 d-md-block bg-light sidebar collapse">
      <div class="position-sticky pt-3">
       
        <h6 class="sidebar-heading d-flex justify-content-between align-items-center px-3 mt-4 mb-1 text-muted">
          <span>管理員</span>
          <a class="link-secondary" href="#" aria-label="Add a new report">
            <span data-feather="plus-circle"></span>
          </a>
        </h6>
        <ul class="nav flex-column mb-2">
          <li class="nav-item">
           
            <router-link  class="nav-link"  to="/admin/products">
            <i class="fas fa-store"></i>
            產品列表
             </router-link>
          </li>
            <li class="nav-item">
              <!-- <a class="nav-link" href="#"> -->
                  <router-link to="/Order_list" class="nav-link">
                  <i class="fas fa-clipboard-list"></i>
                  <span data-feather="file-text"></span>
                  訂單列表
                  </router-link>
                <!-- </a> -->
            </li>
            <li class="nav-item">
              <!-- <a class="nav-link" href="#"> -->
                <router-link to="/Coupon_ticket" class="nav-link">
                <i class="fas fa-tags"></i>
                <span data-feather="file-text"></span>
                優惠卷
                </router-link>
              <!-- </a> -->
            </li>
        </ul>
      </div>
        

      <div class="position-sticky pt-3">
        <h6 class="sidebar-heading d-flex justify-content-between align-items-center px-3 mt-4 mb-1 text-muted">
          <span>模擬功能</span>
          <a class="link-secondary" href="#" aria-label="Add a new report">
            <span data-feather="plus-circle"></span>
          </a>
        </h6>
        <ul class="nav flex-column mb-2">
          <li class="nav-item">
            <!-- <a class="nav-link" href="#"> -->
              <router-link to="/customer_order" class="nav-link">
              <span data-feather="file-text"></span>
              模擬訂單
              </router-link>
            <!-- </a> -->
          </li>
           <li class="nav-item">
            <!-- <a class="nav-link" href="#"> -->
              <router-link to="/Home" class="nav-link">
              <span data-feather="file-text"></span>
              Home
              </router-link>
            <!-- </a> -->
          </li>
        </ul>
      </div>

    </nav>

    </div>
</template>