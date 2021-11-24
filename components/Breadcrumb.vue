<template>
    <section class="page-title-area" :style="{backgroundImage: `url('/images/photos/bg-page-title.jpg')`}">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="page-title-content text-center">
                        <h2 class="title text-white">{{ title }}</h2>
                        <b-breadcrumb :items="items"></b-breadcrumb>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        props: ['items', 'title']
    };
</script>