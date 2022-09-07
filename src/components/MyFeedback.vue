<template>
    <section>
        <div class="container">
            <div class="centred-text">
                <h3 class="myPreTitle">Customer Testimonials</h3>
                <h2>
                    <span class="white">
                        Trusted
                    </span>
                    <span class="bg-green white">
                        Feedback
                    </span>
                </h2>
                <div class="services-parag">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta corrupti architecto sapiente eum tempore officiis blanditiis voluptatum, eos quibusdam fuga pariatur quisquam beatae dicta sequi in optio ratione, animi at?</p>
                </div>
            </div>
            <!-- Possibilità di renderlo un unico componente -->
            <div class="cards">
                <div class="card">
                    <img src="../assets/images/logo-1.png" alt="Logo WooCommerce">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem non et laborum a blanditiis ut libero neque iusto dicta, cumque iure ducimus quibusdam.</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique, molestiae.</p>
                    <div class="quotes">
                        <i class="fa-solid fa-quote-right"></i>
                    </div>
                </div>

                <div class="card centred-card">
                    <img src="../assets/images/logo-2.png" alt="Logo Wordpress">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem non et laborum a blanditiis ut libero neque iusto dicta, cumque iure ducimus quibusdam.</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique, molestiae.</p>
                    <div class="quotes">
                        <i class="fa-solid fa-quote-right"></i>
                    </div>
                </div>
                <div class="card">
                    <img src="../assets/images/logo-3.png" alt="Logo pingdom">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem non et laborum a blanditiis ut libero neque iusto dicta, cumque iure ducimus quibusdam.</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique, molestiae.</p>
                    <div class="quotes">
                        <i class="fa-solid fa-quote-right"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
  
<script>
  export default {
      name: "MyServices",
    
    }
</script>
  
<style scoped lang="scss">
    @import '../styles/vars.scss';
  section {
    height: 600px;
    background-color: #111117;
    .container {
        padding: 60px 0;
        .centred-text {
            text-align: center;
            .services-parag {
                display: flex;
                justify-content: center;
                align-items: center;
                padding-bottom: 40px;
                p {
                    width: 80%;
                    color: #a4a6b3;
                }
            }
        }
        .cards {
            width: 100%;
            display: flex;
            .card {
                background-color: #141419;
                height: 300px;
                width: calc(100% / 3);
                padding: 40px;
                border-radius: 15px;
                position: relative;
                img {
                    width: 50%;
                    padding-bottom: 20px;
                    filter: invert(100%) brightness(200%);
                }
                p {
                    color: #a4a6b3;
                    padding-bottom: 10px;
                }
                .quotes {
                    color:  gray;
                    position: absolute;
                    bottom: 25px;
                    right: 25px;
                    font-size: 25px;
                }
            }
            .centred-card {
                margin: 0 30px;
            }
        }
    }
  }
</style>