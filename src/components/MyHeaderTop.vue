<template>
   <div class="header-top">
        <div class="container">
            <!-- Possibilità di recuperare i valori da un Array per essere riutilizzabili  -->
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
                <div><i class="fa-brands fa-facebook-f"></i></div>
                <div><i class="fa-brands fa-twitter"></i></div>
                <div><i class="fa-brands fa-linkedin-in"></i></div>
            </div>
        </div>
   </div>
  </template>
  
  <script>
  export default {
      name: 'MyHeaderTop',
    }
  </script>
  
  <style scoped lang="scss">
  @import '../styles/vars.scss';
    .header-top {
        height: 40px;
        background-color: $headerBg;
        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: lightgrey;
            i {
                padding-right: 10px;
                font-size: 14px;
            }
            .right {
                display: flex;
                div {
                    padding: 0 15px;
                } 
            }
        }
    }
  </style>