<template>
    <div class="home-default-wrapper">

        <Header />

        <OffCanvasMobileMenu />

        <HeroOne />

        <ServiceOne />

        <AboutOne />

        <CausesOne />

        <DonationStyleOne />

        <FunFactOne />

        <EventsOne />

        <TestimonialOne />

        <BlogStyleOne />

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
            AboutOne: () => import('@/components/AboutOne'),
            CausesOne: () => import('@/components/CausesOne'),
            DonationStyleOne: () => import('@/components/DonationStyleOne'),
            FunFactOne: () => import('@/components/FunFactOne'),
            EventsOne: () => import('@/components/EventsOne'),
            TestimonialOne: () => import('@/components/TestimonialOne'),
            BlogStyleOne: () => import('@/components/BlogStyleOne'),
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


