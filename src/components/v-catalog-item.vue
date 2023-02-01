<template>
    <div>
        <h1></h1>
    </div>
</template>

<script>
import { objectExpression } from '@babel/types';

export default {
    name: 'v-catalog-item',
    props: {
        product_data: {
            type: Object,
            default() {
                return {}
            }
            }
        }
    }
</script>