<!-- <template>
    <div class="user-profile">
      <h1>{{ name }}</h1>
      <p>{{ bio }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'UserProfile',
    props: {
      name: {
        type: String,
        required: true
      },
      bio: {
        type: String,
        default: 'No bio available.'
      }
    }
  }
  </script>
  
  <style scoped>
  .user-profile {
    border: 1px solid #ccc;
    padding: 16px;
    border-radius: 8px;
  }
  </style> -->

  <template>

    <div class="d-flex flex-column flex-shrink-0 p-3 ps-0 bg-gray" style="width: 180px;">
        
        <a href="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto">
          <span class="fs-4"><img src="../assets/img/logo-2.svg" alt=""></span><h6 class="ms-4 mt-2">INGOUDEY</h6>
        </a>
        
        <ul class="nav nav-pills flex-column mb-auto mt-4">
            <li class="nav-item">
            <!-- <img src="../assets/img/sidebar-clicked.svg" alt=""> -->
             <span> <img src="../assets/img/sidebar-home.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page">  Home  </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-order.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Order </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-reviews.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Reviews </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-profile.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Clients </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-company.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Companies </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-trucks.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Trucks </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-brand.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Brands </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-content.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Content Management </a>
          </li> 

          <li class="nav-item ">
            <span><img src="../assets/img/sidebar-permission.svg" alt=""></span>
            <!-- <a href="#" class="nav-link ms-5 text-decoration-none " aria-current="page"> Permission  </a> -->
            <div class="dropdown">
              <a class="btn dropdown-toggle ms-2" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false" type="date">
               Permission
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">A</a></li>
                <li><a class="dropdown-item" href="#">B</a></li>
                <li><a class="dropdown-item" href="#">C</a></li>
              </ul>
            </div>
          </li> 

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-setting.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> System Management </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-translate.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Translation  </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-contact.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none" aria-current="page"> Contact  </a>
          </li>

          <li class="nav-item">
            <span><img src="../assets/img/sidebar-chat.svg" alt=""></span>
            <a href="#" class="nav-link ms-2 text-decoration-none " aria-current="page"> Client Review  </a>
          </li>


        </ul>

        <!-- <div class="dropdown">
          <a href="#" class="d-flex align-items-center link-dark text-decoration-none dropdown-toggle" id="dropdownUser2" data-bs-toggle="dropdown" aria-expanded="false">
            <img src="https://github.com/mdo.png" alt="" width="32" height="32" class="rounded-circle me-2">
            <strong>mdo</strong>
          </a>
          <ul class="dropdown-menu text-small shadow" aria-labelledby="dropdownUser2">
            <li><a class="dropdown-item" href="#">New project...</a></li>
            <li><a class="dropdown-item" href="#">Settings</a></li>
            <li><a class="dropdown-item" href="#">Profile</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Sign out</a></li>
          </ul>
        </div> -->
      </div>


  </template>

<style scoped>
body{
    font-family: 'Poppins',sans-serif;
 }
.dropdown a{
  border: none;
}
li.nav-item:hover{
  background-image: url("../assets/img/sidebar-clicked.svg");
  background-repeat: no-repeat;

}
li.nav-item{
  display: flex;
  justify-content: baseline;
  align-items: center;
margin-bottom: 10px;
  white-space: nowrap; /* Prevent text wrapping */
  overflow: hidden; /* Optional: hide overflowing text */
  text-overflow: ellipsis; /* Optional: add ellipsis for overflow text */

}
li a{
  color: rgb(0, 0, 0);
}
li a:hover{
  color: orange;

}
li img:hover{
background-color: rgb(172, 172, 172);
}

</style>

<script>
export default{
    name :'sidebar'
}
</script>