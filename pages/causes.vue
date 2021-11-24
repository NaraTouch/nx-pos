<template>
    <div class="main-container">

        <Header />

        <OffCanvasMobileMenu />

        <Breadcrumb :items="items" title="Causes" />

        <CausesWrapper />

        <FunFactOne />

        <TestimonialOne />

        <Sponsor />

        <Footer />

        <client-only>
            <back-to-top class="scroll-top" bottom="30px">
                <i class="arrow-top icofont-rounded-up"></i>
                <i class="arrow-bottom icofont-rounded-up"></i>
            </back-to-top>
        </client-only>

    </div>
</template>

<script>
    export default {
        components: {
            Header: () => import('@/components/Header'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            Breadcrumb: () => import('@/components/Breadcrumb'),
            CausesWrapper: () => import('@/components/CausesWrapper'),
            FunFactOne: () => import('@/components/FunFactOne'),
            TestimonialOne: () => import('@/components/TestimonialOne'),
            Sponsor: () => import('@/components/Sponsor'),
            Footer: () => import('@/components/Footer'),
        },

        data() {
            return {
                items: [
                    {
                        text: 'Home',
                        to: "/"
                    },
                    {
                        text: 'Causes',
                        active: true
                    }
                ]
            }
        },

        head() {
            return {
                title: 'Causes'
            }
        },
    };
</script>


