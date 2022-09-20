<template>
<Menu />
<Pcards />

    
</template>


<script>

import Menu from '@/components/Menu.vue'
import Pcards from '@/components/Pcards.vue'

export default {
    name:'FloorView',
    components:{
        Menu,
        Pcards
    }
    
}
</script>