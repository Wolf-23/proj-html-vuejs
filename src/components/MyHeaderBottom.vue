<template>
    <div class="header-bottom">
        <div class="container">
            <!-- Possibilit√† di renderlo un componente  -->
            <nav>
                <div class="brand">
                    <span class="brand-nex">NEX</span>
                    <span class="brand-gen">GEN</span>
                </div>
                <ul>
                    <li v-for="(link, index) in navLinks" :key="index"><a :href="link.link">{{link.text}}</a></li>
                    <li>
                        <a href="#">
                            <i class="fa-solid fa-user"></i>
                        </a>
                    </li>
                    <li class="my-btn"><a href="#">Get in touch</a></li>
                </ul>
            </nav>
            <!-- Possibilit√† di renderlo un componente  -->
            <div class="my-text">
                <h4>Logistic Services</h4>
                <h1>Cargo Transport</h1>
                <p>Fractional or exclusive road cargo transportation to all regions, with small, medium and large vehicles.</p>
                <div>
                    <a href="#" class="my-btn">Get in touch</a>
                </div>
                <div>
                    <a href="#" class="my-empty-btn">Read More</a>
                </div>
            </div>
        </div>
   </div>
</template>
   
<script>
    export default {
        name: 'MyHeaderBottom',
        data() {
            return {
                navLinks: [
                    {
                        text: 'Home',
                        link: '#'
                    },
                    {
                        text: 'About',
                        link: '#'
                    },
                    {
                        text: 'Services',
                        link: '#'
                    },
                    {
                        text: 'Process',
                        link: '#'
                    },
                    {
                        text: 'Testimonials',
                        link: '#'
                    },
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
  @import '../styles/vars.scss';
    .header-bottom {
        background-image: url(../assets/images/bg-9.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        height: 600px;
        position: relative;
        &::after {
            content: '';
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0;
            left: 0;
            background-color: rgba($color: #000000, $alpha: 0.5);
            z-index: 0;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 25px 10px 0;
            z-index: 10;
            position: relative;
            ul {
                list-style: none;
                display: flex;
                align-items: center;
                color: white;
                a {
                    text-decoration: none;
                    text-transform: uppercase;
                    color: white;
                    padding: 0 15px;
                }
            }
        }
        .my-text {
            padding-top: 80px;
            width: 30%;
            z-index: 11;
            position: relative;
            h4 {
                color: $brandColorLight;
                text-transform: uppercase;
                padding-bottom: 10px;
            }
            h1 {
                color: #fff;
                padding-bottom: 10px;
                font-size: 60px;
                font-weight: bolder;
                font-family:Verdana, Tahoma, sans-serif;
                text-transform: uppercase;
            }
            p {
                color: #fff;
                padding-bottom: 50px;
            }
            div {
                padding: 0 15px;
                display: inline-block;
                a {
                    padding: 10px 10px;
                }
            }
        }
    }
</style>