<template>
  <footer class="debug py-5 d-flex align-items-center justify-content-center">
    <div class="border py-4 px-5 text-center">
      <div class="circle animate__swing">
        <i class="fa-solid fa-envelope"></i>
      </div>
      <p class="title">Let's work together.</p>
      <p>&copy; 2022 Designed by Silvia Dugato.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp'
}
</script>

<style lang="scss" scoped >

footer{
  
  .border{
    border: 1px solid black;

    &:hover .circle{
      animation-name: swing-letter;
    }

    .title{
      font-size: 3rem;
      font-weight: bold;
      position: relative;
      &:hover{
        &::after{
          animation-name: change-lenght;
        }
      }


      &::after{
        content: ' ';
        display: table;
        position: absolute;
        height: 5px;
        width: 100%;
        background-color: rgba(0, 0, 0, 0.884);
        animation-duration: 1.5s;
      }
    }

  .circle{
    padding: 15px;
    display: inline-block;
    border: 1px solid black;
    border-radius: 50%;
    animation-duration: 2s;
    .fa-envelope{
      font-size: 2rem;
      
    }
  }
  }

  
  @keyframes change-lenght {
    0%   {width: 90%;}
    50%  {width: 5%;}
    100%  {width: 100%;}
  }

  @keyframes swing-letter {
    0%   {transform: rotate(30deg)}
    25%  {transform: rotate(-30deg)}
    50%  {transform: rotate(15deg)}
    75%  {transform: rotate(-15deg)}
    100% {transform: rotate(0deg)}
  }
}

</style>