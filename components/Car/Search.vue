<script setup>
    const city = ref("");
    const cityError = ref(false);
    // This is usual vue.js way to re-route to a component
    // const router = useRouter();
    // const handleSearch = () => {
    //     router.push(`/city/${city.value}/car`)
    // }
    // This will same underhood of navigateTo component
    const handleSearch = () => {
        if(!city.value){
            return cityError.value = true;
        }
        navigateTo(`/city/${city.value}/car`)
    }
</script>
<!-- Wrap a component inside dir and use it like this syntax- [DirName + ComponentName] -->
<template>
    <div class="font-serif w-[1000px] text-2xl rounded-full bg-white flex justify-between overflow-hidden drop-shadow-2xl mx-auto">
        <input type="text" class="py-3 px-5 w-full text-2xl rounded-full focus:outline-nome" :class="cityError ? 'border-red-500 border' : '' " placeholder="Search by city..." v-model="city">
        <button class="bg-sky-500 px-10 text-white" @click="handleSearch">Search</button>
    </div>
</template>