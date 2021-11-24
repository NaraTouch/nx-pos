<template>
    <div class="blog-page-wrapper">

        <Header />

        <OffCanvasMobileMenu />

        <Breadcrumb :items="items" title="Blog Post" />

        <BlogGridWrapper />

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
            BlogGridWrapper: () => import('@/components/BlogGridWrapper'),
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
                        text: 'Blog',
                        active: true
                    }
                ]
            }
        },

        head() {
            return {
                title: 'Blog'
            }
        },
    };
</script>


