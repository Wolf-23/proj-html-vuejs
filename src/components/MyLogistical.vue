<template>
  <section>
        <div class="logistical-text">
            <h3 class="myPreTitle">How it works in practice</h3>
            <h2>
                <span class="bg-green">
                    Logistical
                </span>
                <span>
                    Procedure
                </span>
            </h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo illum, dolores a minus neque deleniti assumenda.</p>
        </div>
        <div class="cards">
            <div class="card">
                <span class="bg-rounded">01</span>
                <h3>Collection of information</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            </div>
            <div class="card">
                <span class="bg-rounded">02</span>
                <h3>Service Invoice Sending</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            </div>
            <div class="card">
                <span class="bg-rounded">03</span>
                <h3>Withdrawal of Cargo</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            </div>
            <div class="card">
                <span class="bg-rounded">04</span>
                <h3>Transport Customer Order</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            </div>
            <div class="card">
                <span class="bg-rounded">05</span>
                <h3>Successful Delivery</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
            </div>
        </div>
  </section>
</template>

<script>
export default {
    name: 'MyLogistical'
}
</script>

<style lang="scss" scoped>
    @import '../styles/vars.scss';
    section {
        height: 600px;
        background-color: #EEF4ED;
        padding: 90px 0;
        .logistical-text {
            text-align: center;
            p {
                width: 50%;
                margin: 0 auto;
                color: gray;
                padding-top: 15px;
            }
        }
        .cards {
            display: flex;
            text-align: center;
            width: 90%;
            margin: 0 auto;
            padding-top: 50px;
            .card {
                width: calc(100% / 5);
                height: 200px;
                padding: 0 50px;
                span {
                    color: $brandColorDark;
                    margin-bottom: 15px;
                }
                h3 {
                    padding-bottom: 20px;
                }
                p {
                    color: grey;
                }
            }
        }
    }
</style>
