<template>
<div>
    <app-server-status v-for="server in 5" :key="server"></app-server-status> <!-- ignore this error will still compile. Normally for loop requires key-->
</div>
</template>

<script>
    import ServerStat from './ServerStat.vue';
    export default {
        components: {
            'app-server-status': ServerStat
        }
    }
</script>