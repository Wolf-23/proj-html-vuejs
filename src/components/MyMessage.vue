<template>
  <section>
    <div class="container">
        <div class="left">
            <h3 class="myPreTitle">Send a Message</h3>
            <h2>
                <span>
                    Get in 
                </span>
                <span class="bg-green">
                    Touch
                </span>
            </h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Temporibus, voluptatem.</p>
            <form>
                <div class="input-name">
                    <input type="text" placeholder="Name">
                </div>
                <div  class="input-email" >
                    <input type="text" placeholder="Email">
                </div>
                <div class="input-phone" >
                    <input type="text" placeholder="Phone">
                </div>
                <div class="form-select">
                    <select>
                        <option>More Info</option>
                        <option>More Info 2</option>
                        <option>More Info 3</option>
                    </select>
                </div>
                <textarea rows="7" placeholder="Message"></textarea>
                <a class="my-btn" href="#">Send</a>
            </form>

        </div>
        <div class="right">
            <h3>Example Inc.</h3>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Iusto, perspiciatis?</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Iusto, perspiciatis?</p>
            <div class="phone-number">
                <i :class="contacts.phone.icon"></i>
                <span>{{contacts.phone.text}}</span>
            </div>
            <div class="email">
                <i :class="contacts.email.icon"></i>
                <span>{{contacts.email.text}}</span>
            </div>
            <div class="maps">
                <i :class="contacts.maps.icon"></i>
                <span>{{contacts.maps.text}}</span>
            </div>
            <a href="#" class="my-empty-btn">View Map</a>
        </div>
    </div>
  </section>
</template>

<script>
    export default {
        name: 'MyMessage',
        props: {
            contacts: Object
        }
    }
</script>

<style lang="scss" scoped>
    @import '../styles/vars.scss';
    section {
        background-color: #fff;
        height: 600px;
        .container {
            padding: 70px 0;
            display: flex;
            .left {
                width: 70%;
                p {
                    font-size: 13px;
                    color: gray;
                    padding-bottom: 20px;
                    padding-top: 20px;
                }
                form {
                    width: 80%;
                    display: flex;
                    flex-wrap: wrap;
                    div {
                        width: 50%;
                        input, select {
                            width: calc(100% - 10px);
                            margin-bottom: 10px;
                           
                        }
                        select {
                            color: gray;
                        }
                    }
                    textarea {
                        width: calc(100% - 10px);
                        resize: none;
                    }
                    input, select, textarea {
                        padding: 10px;
                        background-color: rgb(230, 230, 230);
                        border: none;
                        border-radius: 5px;
                    }
                    a {
                        margin-top: 20px;
                        padding: 10px 25px;
                    }
                }
            }
            .right {
                width: 30%;
                h3, p {
                    margin-bottom: 15px;
                }
                p {
                    color: gray;
                    font-size: 13px;
                }
                .phone-number, .email, .maps {
                    padding-bottom: 20px;
                    span {
                        color: $brandColorDark;
                    }
                    i {
                        display: inline-block;
                        margin-right: 10px;
                        color: $brandColorDark;
                        font-weight: bold;
                        background-color: rgba(3, 131, 132, 0.1);
                        border-radius: 50%;
                        height: 35px;
                        width: 35px;
                        line-height: 35px;
                        text-align: center;
                    }
                }
                a.my-empty-btn {
                    color: $brandColorDark;
                    font-size: 12px;
                    padding: 10px 15px;
                }
            }
        }
    }
</style>