<template>
    <div>
        <h1>Каталог</h1>
        <div class="v-catalog__list">
            <v-catalog-item 
            v-for="product in products" 
            :key="product.article"
            :product_data="product"
            />
    
        </div>
    </div>
</template>

<script>
import vCatalogItem from './v-catalog-item.vue';

export default {
    name: 'v-catalog',
    components: {
        vCatalogItem
    },
    props: {},
    data() {
        return {
            products: [
                {
                    image: '1.jpg',
                    name: 'tovar 1',
                    price: '100',
                    article: 't1',
                    available: true
                },
                {
                    image: '2.jpg',
                    name: 'tovar 2',
                    price: '200',
                    article: 't2',
                    available: true
                },
            ]
        }
    }
}
</script>