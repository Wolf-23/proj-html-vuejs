<template>
  <section>
    <div class="container"> 
        <h3 class="myPreTitle">What Are We Doing</h3>
        <h2>
            <span class="bg-green white">
                Results
            </span>
            <span class="white">
                in Numbers
            </span>
        </h2>
        <div class="cards">
            <div class="card">
                <span>128</span>
                <h4>Certifications</h4>
            </div>
            <div class="card">
                <span>230</span>
                <h4>Employees</h4>
            </div>
            <div class="card">
                <span>517</span>
                <h4>Customers</h4>
            </div>
            <div class="card">
                <span>94</span>
                <h4>Countries Served</h4>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
    export default {
        name: 'MyResults'
    }   
</script>

<style lang="scss" scoped>
    @import '../styles/vars.scss';
    section {
        height: 400px;
        background-image: url(../assets/images/bg-10.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        .container {
            padding: 70px 0;
            text-align: center;
            .cards {
                padding-top: 40px;
                display: flex;
                justify-content: space-between;
                width: 60%;
                margin: 0 auto;
                .card {
                    color: #fff;
                    padding-top: 50px;
                    span {
                        color: $brandColorLight;
                        display: inline-block;
                        font-size: 28px;
                        font-weight: bold;
                        padding-bottom: 10px;
                    }
                    h4 {
                        font-size: 18px;
                    }
                }
            }
        }
    }
</style>