<template>
    <div class="home-default-wrapper">

        <Header />

        <OffCanvasMobileMenu />

        <HeroOne />

        <ServiceOne />

        <CausesOne />

        <FunFactOne />

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
            HeroOne: () => import('@/components/HeroOne'),
            ServiceOne: () => import('@/components/ServiceOne'),
            CausesOne: () => import('@/components/CausesOne'),
            FunFactOne: () => import('@/components/FunFactOne'),
            Sponsor: () => import('@/components/Sponsor'),
            Footer: () => import('@/components/Footer'),
        },

        head() {
            return {
                title: 'Home'
            }
        },
    };
</script>


