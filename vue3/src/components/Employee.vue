<script>
                export default {
                    props: ['name', 'surn','age'],
                    data() {
                        return {
                            
                        }
                    }
                }
</script>

<template>
<p class="pstyle">{{ name }}</p>
<p class="pstyle">{{ surn }}</p>
<p class="pstyle">{{ age }}</p>
</template>