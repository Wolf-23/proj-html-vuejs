<template>
  <section>
    <div class="container">
        <div class="logistical-text">
            <h3>How it works in practice</h3>
            <h2>
                <span class="bg-green">
                    Logistical
                </span>
                <span>
                    Procedure
                </span>
            </h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo illum, dolores a minus neque deleniti assumenda. Aut reprehenderit ipsa eos dolor harum a repellat maxime nostrum quod. In, eaque esse.</p>
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
        height: 500px;
        background-color: #EEF4ED;
        .container {
            padding: 90px 0;
            .logistical-text {
                text-align: center;
                h3 {
                    text-transform: uppercase;
                    font-size: 14px;
                    padding-bottom: 20px;
                    color: $brandColorLight;
                }
                h2 {
                    font-size: 35px;
                    padding-bottom: 20px;
                }
                p {
                    width: 60%;
                    margin: 0 auto;
                    color: gray;
                }
            }
        }
    }
</style>>
