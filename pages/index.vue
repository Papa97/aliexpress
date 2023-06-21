<script setup>
import MainLayout from '~/layouts/MainLayout.vue';

const products = [
    {
        id: 1,
        title: 'title 1',
        description: 'desc 1',
        url: 'https://picsum.photos/id/7/800/800',
        price: 999,
    },
    {
        id: 2,
        title: 'title 2',
        description: 'desc 2',
        url: 'https://picsum.photos/id/71/800/800',
        price: 999,
    },
    {
        id: 3,
        title: 'title 3',
        description: 'desc 3',
        url: 'https://picsum.photos/id/72/800/800',
        price: 999,
    },
    {
        id: 4,
        title: 'title 4',
        description: 'desc 4',
        url: 'https://picsum.photos/id/73/800/800',
        price: 999,
    },
    {
        id: 5,
        title: 'title 5',
        description: 'desc 5',
        url: 'https://picsum.photos/id/74/800/800',
        price: 999,
    },
    {
        id: 6,
        title: 'title 6',
        description: 'desc 6',
        url: 'https://picsum.photos/id/75/800/800',
        price: 999,
    },
    {
        id: 7,
        title: 'title 7',
        description: 'desc 7',
        url: 'https://picsum.photos/id/76/800/800',
        price: 999,
    },
    {
        id: 8,
        title: 'title 8',
        description: 'desc 8',
        url: 'https://picsum.photos/id/77/800/800',
        price: 999,
    },
    {
        id: 9,
        title: 'title 9',
        description: 'desc 9',
        url: 'https://picsum.photos/id/78/800/800',
        price: 999,
    },
    {
        id: 10,
        title: 'title 10',
        description: 'desc 10',
        url: 'https://picsum.photos/id/79/800/800',
        price: 999,
    },
];
</script>

<style lang="scss" scoped></style>

<template>
    <MainLayout>
        <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
            <div
                class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-col-4 gap-4"
            >
                <div v-if="products" v-for="product in products" :key="product">
                    <!-- {{ product }} -->
                    <ProductComponent :product="product" />
                </div>
            </div>
        </div>
    </MainLayout>
</template>
