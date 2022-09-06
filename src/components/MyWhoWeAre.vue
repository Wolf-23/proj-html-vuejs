<template>
    <section>
      <div class="container">
        <div class="left">
            <h3>Who We Are</h3>
            <h2>
                <span class="bg-green">
                    <i class="fa-regular fa-gem"></i>
                    Excellence
                </span>
                <span>
                    in Transport
                </span>
            </h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est at atque, ex quaerat suscipit similique blanditiis dignissimos iure voluptatum eligendi corporis quos porro aliquid et, iste laboriosam fugiat commodi aperiam!</p>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fugiat quas repudiandae assumenda rerum expedita debitis velit earum quod officiis accusantium vel veniam deleniti quam dolor laboriosam excepturi culpa, consequuntur non!</p>
            <blockquote>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit aut labore molestias, nulla laboriosam vitae voluptate numquam.
            </blockquote>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            <ul>
                <li>Lorem ipsum dolor sit amet</li>
                <li>Lorem ipsum dolor sit amet</li>
                <li>Lorem ipsum dolor sit amet</li>
                <li>Lorem ipsum dolor sit amet</li>
                <li>Lorem ipsum dolor sit amet</li>
            </ul>
        </div>
        <div class="right">
            <h3>Vehicle Types</h3>
            <!-- Possibilità di renderlo un componente  -->
            <div class="truck">
                <img class="img-truck" src="../assets/images/truck-1.png" alt="Veicolo">
                <div class="truck-features">
                    <h3>Light</h3>
                    <h4>Max Weight 1200 Kg</h4>
                </div>
            </div>
            <div class="truck">
                <img class="img-truck" src="../assets/images/truck-1.png" alt="Veicolo">
                <div class="truck-features">
                    <h3>Medium</h3>
                    <h4>Max Weight 6000 Kg</h4>
                </div>
            </div>
            <div class="truck">
                <img class="img-truck" src="../assets/images/truck-1.png" alt="Veicolo">
                <div class="truck-features">
                    <h3>Heavy</h3>
                    <h4>Max Weight 24000 Kg</h4>
                </div>
            </div>
            <h3>Certificatons</h3>
            <img class="certification" src="../assets/images/certificate.png" alt="Certificate">
            <img class="certification" src="../assets/images/certificate.png" alt="Certificate">
        </div>
      </div>
    </section>
</template>
  
<script>
    export default {
      name: 'MyWhoWeAre'
    }
</script>
<style scoped lang="scss">
    @import '../styles/vars.scss';
    section {
        background-color: #fff;
        height: 600px;
        .container {
            display: flex;
            padding: 70px 0;
            .left{
                width: 70%;
                h3 {
                    color: $brandColorLight;
                    padding-bottom: 10px;
                    text-transform: uppercase;
                    font-size: 14px;
                }
                h2 {
                    font-size: 35px;
                    padding-bottom: 10px;
                    span {
                        padding: 0 5px;
                    }
                }
                p {
                    margin-bottom: 20px;
                    color: grey;
                }
                blockquote {   
                    padding: 10px 30px;
                    color: grey;
                    border-left: 4px solid rgba(3, 131, 132, 0.3);
                    margin-bottom: 20px;
                    font-style: italic;
                }
                ul {
                    padding-left: 20px;
                    color: grey;
                    li {
                        padding: 3px 0;
                    }
                }
            }
            .right {
                width: 30%;
                padding-left: 50px;
                h3 {
                    font-size: 22px;
                    margin-bottom: 10px;
                }
                .truck {
                    display: flex;
                    align-items: center;
                    padding-bottom: 10px;
                    border-bottom: 1px solid grey;
                    margin-bottom: 10px;
                    .img-truck {
                        width: 90px;
                        background-color:rgba(3, 131, 132, 0.3);
                        border-radius: 5px;
                        padding: 10px;
                    }
                    .truck-features {
                        padding-left: 30px;
                        h4 {
                            color: grey;
                            font-weight: 100;
                        }
                    }
                }
                .certification {
                    width: 120px;
                    margin: 0 10px;
                }
            }
            
        } 
    }
</style>