<template>
    <section>
      <div class="container">
        <div>
          <p>Enjoy the low price. We are tracking any intention of piracy</p>
        </div>
        <div>
          <span>
            <i class="fa-regular fa-copyright"></i>
          </span>
          <span>
            2020 NEXTGEN is Proudly Powered by <span class="text-green">Codings</span>
          </span>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
      name: 'MyFooterBottom'
    }
  </script>
  <style lang="scss" scoped>
    @import '../styles/vars.scss';
    section {
      height: 80px;
      background-color: #000;
      .container {
        display: flex;
        height: 100%;
        justify-content: space-between;
        align-items: center;
        div {
          color: lightgray;
          font-size: 13px;
          span.text-green {
            color: $brandColorLight;
          }
        }
      }
    }
  </style>