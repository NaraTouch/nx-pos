<template>
    <section class="causes-area causes-default-area">
        <div class="container">
            <div class="row mtn-30">
                <div class="col-md-6 col-lg-4 mt-30" v-for="(pricing, index) in pricingData" :key="index">
                    <div class="causes-item">
                        <div class="thumb">
                            <img :src="pricing.imgSrc" :alt="pricing.title">
                        </div>
                        <div class="content">
                            <ul class="donate-info">
                                <li class="info-item" v-for="(info, index) in pricing.infoList" :key="index">
                                    <span class="info-title">{{ info.infoTitle }}:</span>
                                    <span class="amount">{{ info.amount }}</span>
                                </li>
                            </ul>
                            <h4 class="title">
                                <n-link to="/pricing-details">{{ pricing.title }}</n-link>
                            </h4>
                            <p>{{ pricing.desc }}</p>
                        </div>
                        <div class="causes-footer">
                            <div class="admin">
                                
                            </div>
                            <n-link to="/pricing" class="btn-theme btn-border-gradient gray-border btn-size-md">
                                <span>
                                    Buy Now
                                    <img class="icon icon-img" src="/images/icons/arrow-line-right-gradient.png" alt="Icon">
                                </span>
                            </n-link>
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
                pricingData: [
                    {
                        imgSrc: "/images/causes/01.jpg",
                        title: "NX POS System.",
                        desc: "Lorem Ipsum is simply dummy text of the industry's since the unknown.",
                        infoList: [
                            {
                                infoTitle: "Trial",
                                amount: "7 Days"
                            },
                            {
                                infoTitle: "Monthly",
                                amount: "$ 69.99"
                            },
                            {
                                infoTitle: "Yearly",
                                amount: "$ 800"
                            }
                        ]
                    },
                    {
                        imgSrc: "/images/causes/02.jpg",
                        title: "Ecommerce Owner",
                        desc: "Lorem Ipsum is simply dummy text of the industry's since the unknown.",
                        infoList: [
                            {
                                infoTitle: "Trial",
                                amount: "14 Days"
                            },
                            {
                                infoTitle: "Monthly",
                                amount: "$ 49.99"
                            },
                            {
                                infoTitle: "Yearly",
                                amount: "$ 550"
                            }
                        ]
                    },
                    {
                        imgSrc: "/images/causes/03.jpg",
                        title: "Feature and Addon",
                        desc: "Lorem Ipsum is simply dummy text of the industry's since the unknown.",
                        infoList: [
                            {
                                infoTitle: "Trial",
                                amount: "14 Days"
                            },
                            {
                                infoTitle: "Monthly",
                                amount: "$ 1.99"
                            },
                            {
                                infoTitle: "Yearly",
                                amount: "$ 10.99"
                            }
                        ]
                    }
                ]
            }
        },
    };
</script>