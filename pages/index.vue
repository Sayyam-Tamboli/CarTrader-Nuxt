<!-- in Nuxt
if you call a component from components dir to a page dir component
it do imports by itself
<script setup>
import NavBar from '../components/NavBar.vue'
</script> 
-->
<script setup>
    useHead({
        title: "CarTrader",
    });
</script>
<template>
    <div>
        <!-- Wrap a component inside dir and use it like this syntax- [DirName + ComponentName] -->
        <CarHero/>
    </div>
</template>