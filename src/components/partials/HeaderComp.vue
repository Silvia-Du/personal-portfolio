<template>
  <header>
    <div class="px-4 py-3 d-flex justify-content-between">

      <img src="../../assets/img/logo.png" alt="logo-sd">

      <div class="d-flex align-items-center">
        <i class="fa-regular fa-moon"></i>
        <!-- hamburger -->
        <div class="hamburger ms-3">
          <div class="up"></div>
          <div class="bottom"></div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComp'
}
</script>

<style lang="scss" scoped >
@import '../../assets/style/vars';

header{
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 999;
  img{
    width: 50px;
  }

  .fa-moon{
    font-size: 1.7rem;
  }

  .hamburger{
    position: relative;
    width: 27px;
    height: 18px;
    &:active .up{
        transform: rotate(-40deg);
        top: 6px;
      }
    &:active .bottom{
        transform: rotate(38deg);
        bottom: 7px;
      }
    .up, .bottom{
      position: absolute;
      width: 100%;
      height: 2px;
      border-radius: 3px;
      background-color: $blackText;
      transition: all 0.2s;
    }

    .up{
      margin-bottom: 10px;
      top: 0;
      left: 0;
    }
    .bottom{
      bottom: 0;
      left: 0;
    }
  }
}

</style>