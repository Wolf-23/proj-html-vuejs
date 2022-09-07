<template>
    <section>
        <div class="container">
            <div class="cards">
                <div class="card-text">
                    <div class="brand">
                        <span class="brand-nex">NEX</span>
                        <span class="brand-gen">GEN</span>
                    </div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores, aut.</p>
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
                    <a href="#" class="my-empty-btn">get in Touch</a>
                </div>
                <div class="card">
                    <h3>{{information.about.title}}</h3>
                    <ul v-for="(text, index) in information.about.lists" :key="index">
                        <li>
                            <span>
                                <i :class="text.icon"></i>
                            </span>
                            <span>{{text.text}}</span>
                        </li>
                    </ul>
                </div>
                <div class="card">
                    <h3>{{information.transport.title}}</h3>
                    <ul v-for="(text, index) in information.transport.lists" :key="index">
                        <li>
                            <span>
                                <i :class="text.icon"></i>
                            </span>
                            <span>{{text.text}}</span>
                        </li>
                    </ul>
                </div>
                <div class="card">
                    <h3>{{information.support.title}}</h3>
                    <ul v-for="(text, index) in information.support.lists" :key="index">
                        <li>
                            <span>
                                <i :class="text.icon"></i>
                            </span>
                            <span>{{text.text}}</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
  </template>
  
  <script>
  export default {
      name: 'MyFooterTop',
      props: {
            contacts: Object
        },
        data() {
            return {
                information: {
                    about: {
                        title: 'About',
                        lists: [
                            {
                                text: 'The Company',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Institutional',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Social & Events',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Innovation',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Environment',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Technology',
                                icon: 'fa-solid fa-chevron-right'
                            },
                        ]
                    },
                    transport: {
                       title: 'Transports',
                       lists: [
                            {
                                text: 'Industrialized',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Chemical',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Packaged Liquids',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Construction',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Laminated Wood',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'And others',
                                icon: 'fa-solid fa-chevron-right'
                            },
                       ]
                    },
                    support: {
                       title: 'Support',
                       lists: [
                            {
                                text: 'Responsability',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Theme of Use',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'About Cookies',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Privacy Policy',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Accessibility',
                                icon: 'fa-solid fa-chevron-right'
                            },
                            {
                                text: 'Informations',
                                icon: 'fa-solid fa-chevron-right'
                            },
                       ]
                    } 
                }
            }
        }

    }
  </script>
  
  <style lang="scss" scoped>
    @import '../styles/vars.scss';
    section {
        background-color: #111117;
        height: 500px;
        .container {
            padding: 90px 0;
            .cards {
                display: flex;
                justify-content: space-between;
                .card-text {
                    .brand {
                        margin-bottom: 30px;
                    }
                    p {
                        padding-bottom: 20px;
                        font-size: 14px;
                        color: lightgray;
                    }
                    .phone-number, .email, .maps {
                        padding-bottom: 15px;
                        color: lightgray;
                        i {
                            margin-right: 10px;
                        }
                    }
                    a.my-empty-btn {
                        margin-top: 20px;
                        display: inline-block;
                        padding: 10px 15px;
                    }
                }
                .card-text, .card {
                    width: calc(100% / 4 - 20px);
                }
                .card {
                    background-color: #141419;
                    padding: 25px;
                    border-radius: 15px;
                    h3 {
                        margin-bottom: 30px;
                        color: #fff;
                    }
                    ul {
                        list-style: none;
                        color: lightgray;
                        li {
                            margin-bottom: 15px;
                            font-size: 14px;
                            i {
                                margin-right: 10px;
                            }
                        }
                    }
                }
            }
        }
    }
</style>