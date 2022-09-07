<template>
    <section>
        <div class="container">
            <h3 class="myPreTitle">Road Transport</h3>
            <h2>
                <span class="white">
                    Main
                </span>
                <span class="bg-green white">
                    Services
                </span>
            </h2>
            <div class="services-parag">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta corrupti architecto sapiente eum tempore officiis blanditiis voluptatum, eos quibusdam fuga pariatur quisquam beatae dicta sequi in optio ratione, animi at?</p>
                <a href="#" class="my-empty-btn">SEE ALL</a>
            </div>
            <!-- Possibilità di renderlo un unico componente -->
            <div class="cards">
                <div class="card">
                    <div class="icon-bg bg-rounded">
                        <i class="fa-solid fa-truck-ramp-box"></i>
                    </div>
                    <h4>Tecnology</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem non et laborum a blanditiis ut libero neque iusto dicta, cumque iure ducimus quibusdam nisi minus qui incidunt accusamus reiciendis id.</p>
                    <div class="arrow">
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                </div>

                <div class="card centred-card">
                    <div class="icon-bg bg-rounded">
                        <i class="fa-solid fa-temperature-low"></i>
                    </div>
                    <h4>Reefer Cargo</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem non et laborum a blanditiis ut libero neque iusto dicta, cumque iure ducimus quibusdam nisi minus qui incidunt accusamus reiciendis id.</p>
                    <div class="arrow">
                        <i class="fa-solid fa-arrow-right"></i>
                    </div>
                </div>
                <div class="card">
                    <div class="icon-bg bg-rounded">
                        <i class="fa-solid fa-boxes-stacked"></i>
                    </div>
                    <h4>Dry Cargo</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem non et laborum a blanditiis ut libero neque iusto dicta, cumque iure ducimus quibusdam nisi minus qui incidunt accusamus reiciendis id.</p>
                    <div class="arrow">
                        <i class="fa-solid fa-arrow-right"></i>
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
        padding: 70px 0;
        .services-parag {
            display: flex;
            align-items: center;
            padding-bottom: 40px;
            p {
                width: 80%;
                color: #fff;
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
                .icon-bg {
                    width: 50px;
                    height: 50px;
                    line-height: 25px;
                    padding: 10px;
                    font-size: 25px;
                    color: $brandColorLight;
                }
                h4 {
                    padding: 20px 0;
                    color: #fff;
                    font-size: 24px;
                }
                p {
                    color: #fff;
                }
                .arrow {
                    color:  $brandColorLight;
                    position: absolute;
                    top: 50px;
                    right: 50px;
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