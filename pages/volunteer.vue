<template>
    <div class="volunteer-page-wrapper">

        <Header />

        <OffCanvasMobileMenu />

        <Breadcrumb :items="items" title="Become Volunteer" />

        <VolunteerForm />

        <TeamTwo />

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
            Breadcrumb: () => import('@/components/Breadcrumb'),
            VolunteerForm: () => import('@/components/VolunteerForm'),
            TeamTwo: () => import('@/components/TeamTwo'),
            FunFactOne: () => import('@/components/FunFactOne'),
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
                        text: 'Volunteer',
                        active: true
                    }
                ]
            }
        },

        head() {
            return {
                title: 'Volunteer'
            }
        },
    };
</script>


