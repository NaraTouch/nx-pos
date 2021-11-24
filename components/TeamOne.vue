<template>
    <section class="team-area team-fluid-area">
        <div class="container">
            <div class="row">
                <div class="col-lg-6 offset-lg-3 col-xl-4 offset-xl-0">
                    <div class="section-title">
                        <h5 class="subtitle line-theme-color mb-7">Volunteer Team</h5>
                        <h2 class="title title-style">Volunteer Team of Givest. <img class="img-shape" src="/images/shape/3.png" alt="Image-Givest"></h2>
                        <div class="desc">
                            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry's standard dummy text ever since and unknown printer took scrambled it make specimen book.</p>
                            <n-link to="/volunteer" class="btn-theme btn-gradient btn-slide">Join Now <img class="icon icon-img" src="/images/icons/arrow-line-right2.png" alt="Icon"></n-link>
                        </div>
                    </div>
                </div>
                <div class="col-xl-8">
                    <div class="team-member-items">
                        <div class="team-slider-container">
                            <swiper :options="teamSlider">
                                <div class="swiper-slide team-member" v-for="(member, index) in teamMembers" :key="index">
                                    <div class="thumb">
                                        <img :src="member.imgSrc" :alt="member.name">
                                        <div class="social-icons">
                                            <a :href="list.url" v-for="(list, index) in member.socialLink" :key="index">
                                                <i :class="list.icon"></i>
                                            </a>
                                        </div>
                                    </div>
                                    <div class="content">
                                        <div class="member-info">
                                            <h4 class="name"><a href="#">{{ member.name }}</a></h4>
                                            <h6 class="designation">{{ member.designation }}</h6>
                                        </div>
                                    </div>
                                </div>
                            </swiper>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                teamSlider: {
                    autoplay: true,
                    loop: true,
                    speed: 1500,
                    slidesPerView: 3,
                    spaceBetween : 30,
                    breakpoints: {
                        1200:{
                            slidesPerView : 3
                        },

                        768:{
                            slidesPerView : 3
                        },

                        320:{
                            slidesPerView : 1
                        }
                    }
                },

                teamMembers: [
                    {
                        imgSrc: "/images/team/1.jpg",
                        name: "Harvey Harrington",
                        designation: "Senior Designer",
                        socialLink: [
                            {
                                icon: "icofont-facebook",
                                url: "#"
                            },
                            {
                                icon: "icofont-skype",
                                url: "#"
                            },
                            {
                                icon: "icofont-twitter",
                                url: "#"
                            }
                        ]
                    },
                    {
                        imgSrc: "/images/team/2.jpg",
                        name: "Alejandra Bobbitt",
                        designation: "Senior Volunteer",
                        socialLink: [
                            {
                                icon: "icofont-facebook",
                                url: "#"
                            },
                            {
                                icon: "icofont-skype",
                                url: "#"
                            },
                            {
                                icon: "icofont-twitter",
                                url: "#"
                            }
                        ]
                    },
                    {
                        imgSrc: "/images/team/3.jpg",
                        name: "Sherika Hankins",
                        designation: "Senior Developer",
                        socialLink: [
                            {
                                icon: "icofont-facebook",
                                url: "#"
                            },
                            {
                                icon: "icofont-skype",
                                url: "#"
                            },
                            {
                                icon: "icofont-twitter",
                                url: "#"
                            }
                        ]
                    }
                ]
            }
        },
    };
</script>