<template>

    <Menu />
    <Inventory />
</template>


<script>
import Menu from '@/components/Menu.vue'
import Inventory from '@/components/Inventory.vue'
export default {
    name:'InventoryView',
    components: {
        Inventory,
        Menu
    }
}
</script>