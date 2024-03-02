<!-- in Nuxt
if you call a component from components dir to a page dir component
it do imports by itself
<script setup>
import NavBar from '../components/NavBar.vue'
</script> 
-->
<template>
    <div>
        <NavBar/>
        <!-- Wrap a component inside dir and use it like this syntax- [DirName + ComponentName] -->
        <CarHero/>
    </div>
</template>