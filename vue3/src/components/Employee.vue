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
<ul>
    <li v-for="elem in name">{{ elem }}</li>
</ul>
</template>