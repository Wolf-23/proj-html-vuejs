<template>
   <div class="header-top">
        <div class="container">
            <div class="open">
                <i class="fa-solid fa-clock"></i>
                <span>Open Hours: Mon - Sat - 9:00 - 18:00</span>
            </div>
            <div class="right">
                <div class="phone-number">
                    <i class="fa-solid fa-phone"></i>
                    <span>+1 (305) 1234-5678</span>
                </div>
                <div class="email">
                    <i class="fa-solid fa-envelope"></i>
                    <span>hello@example.com</span>
                </div>
            </div>
        </div>
   </div>
  </template>
  
  <script>
  export default {
      name: 'MyHeaderTop'
  }
  </script>
  
  <style scoped lang="scss">
    .header-top {
        height: 30px;
        background-color: #21333E;
        .container {
            height: 100%;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
            i {
                padding-right: 5px;
            }
            .right {
                display: flex;
            }
        }
    }
  </style>