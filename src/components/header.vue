
<template>

        <p class="title m-0 p-0 ms-3"> Dashboard review </p> 
        <div class="menu-img me-3">
            <a href="#" class="me-2 img-1"><img src="../assets/img/header-notification.svg" alt=""></a>
            <div id="line"></div>
            <div class="dropdown">
                <a class="btn border:none dropdown-toggle ms-2" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                    <a href="#" ><img src="../assets/img/logo-2.svg" alt=""> iNGOUDE COMPANY </a>
                </a>
                <ul class="dropdown-menu" >
                  <li><a class="dropdown-item" href="#">User 1</a></li>
                  <li><a class="dropdown-item" href="#">User 2</a></li>
                  <li><a class="dropdown-item" href="#">User 3</a></li>
                </ul>
                
              </div>
            <!-- <a href="#" ><img src="../assets/img/logo-2.svg" alt=""> iNGOUDE COMPANY </a> -->
        </div>

</template>

<style>
#line{
    border-left: 2px solid #353535 ;
    height: 40px;
    border-radius: 40px;
    opacity: 10%;
    margin: 5px;

}
.title , .menu-img{
    display: flex;
    align-items: center;
}
.title{
    font-family: 'Poppins',sans-serif;
    font-weight: bold;

}

a{
    color: #353535;
    text-decoration: none;
}
</style>
 
<script>
export default {
    name : 'header'
}
</script>