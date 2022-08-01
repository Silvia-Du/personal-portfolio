<template>
  <div class="debug">
    
      <!-- about -->
      <div class="about">

        <div class="container py-5">
          <div class="row py-5">
            <div class="col-12 col-md-6 col-left">
              <img  src="../assets/img/MePlaceholder.png" alt="sd-img">
            </div>
            <div class="col-12 col-md-6 col-right d-flex justify-content-center flex-column">
              <p class="title">Silvia Dugato</p>
              <p class="subtitle">Jr. Full Stack Web Developer</p>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Animi laboriosam ab architecto dolorum quos, velit magnam temporibus ratione ex ipsa ullam explicabo. Sequi, quaerat deserunt! Quam consectetur quo commodi molestiae expedita omnis repellendus nesciunt ab earum. Iusto molestias assumenda quasi itaque, iste reiciendis velit optio dolorum ullam, perferendis, ut facilis!</p>
            </div>
          </div>
      </div>
        
      </div>
      <!-- servizi -->
      <div class="services debug container-fluid py-5">
        <div class="row">
          <div class="col-12 col-md-3 debug">
            
          </div>
          <div class="col-12 col-md-3 debug">b</div>
          <div class="col-12 col-md-3 debug">a</div>
          <div class="col-12 col-md-3 debug">b</div>
        </div>
            
            
        
      </div>
      <!-- linguaggi -->
      <div class="dev-language debug py-5 container">
        <p class="title my-5 animate__animated animate__fadeInLeft">Ho lavorato con</p>
        
        <div class="d-flex justify-content-around align-items-center flex-wrap my-5">
          <i class="fa-brands fa-html5 animate__animated animate__fadeInTopRight"></i>
          <i class="fa-brands fa-css3-alt animate__animated animate__fadeInBottomLeft"></i>
          <i class="fa-brands fa-vuejs animate__animated animate__fadeInTopLeft"></i>
          <i class="fa-brands fa-git-alt animate__animated"></i>
          <i class="fa-brands fa-js animate__animated animate__fadeInLeft"></i>
          <i class="fa-brands fa-bootstrap animate__animated"></i>
          <i class="fa-brands fa-sass animate__animated animate__fadeInBottomLeft"></i>
          <i class="fa-brands fa-laravel animate__animated animate__fadeInTopLeft"></i>
          <i class="fa-brands fa-php animate__animated animate__fadeInTopRight"></i>
          <img src="../assets/img/vsIcon.png" alt="vs-icon">
        </div>

      </div>
    
  </div>
  
</template>

<script>
export default {
  name: 'AboutComp'
}
</script>

<style lang="scss" scoped >

@import '../assets/style/vars';
@import '../assets/style/mixin';

.about{
  background-image: url(../assets/img/aboutBg.png);
  @include backGroundRole();

  .col-left{
    img{
      width: 100%;
    }
  }
  .title{
    @include sectionTitle();
  }
  .subtitle{
    @include sectionSubtitle();
  }
  
}

.services{
  min-height: 300px;
  .serv-col{
    min-height: 400px;
  }
}

.dev-language{
  background-color: $bgLightGray;

  .title{
    @include sectionTitle();
    color: $blackText;
  }
  .fa-brands{
    font-size: 3rem;
    color: $iconColor;
  }
  img{
    width: 50px;
  }
}


</style>