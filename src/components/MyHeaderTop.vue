<template>
   <div class="header-top">
        <div class="container">
            <!-- Possibilità di recuperare i valori da un Array per essere riutilizzabili  -->
            <div class="open">
                <i :class="contacts.clock.icon"></i>
                <span>{{contacts.clock.text}}</span>
            </div>
            <div class="right">
                <div class="phone-number">
                    <i :class="contacts.phone.icon"></i>
                    <span>{{contacts.phone.text}}</span>
                </div>
                <div class="email">
                    <i :class="contacts.email.icon"></i>
                    <span>{{contacts.email.text}}</span>
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
      props: {
            contacts: Object
        }
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
            font-size: 14px;
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