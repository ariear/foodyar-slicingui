<template>
<div class="font-pupylinux pb-28">

    <div class="text-center">
        <p class="font-normal text-xl text-[#8B8BA5] mb-2">Watch Now</p>
        <p class="font-bold text-[32px] text-[#272042] mb-7">Special to Try</p>
    </div>
    <div class="font-normal text-base md:text-xl flex justify-center items-center text-center">
        <p class="mx-4 text-[#F7C531] relative">Healthy Food <span class="border border-[#F7C531] w-[50%] absolute mx-auto left-0 right-0 -bottom-2"></span></p>
        <p class="mx-4">Lunch</p>
        <p class="mx-4">Vege Desert</p>
        <p class="mx-4">Shake</p>
    </div>
    <div class="container mx-auto grid md:grid-cols-2 lg:grid-cols-4 gap-y-8 lg:gap-y-0 justify-items-center mt-16">
        <div v-for="(menu, index) in menusehat" :key="index" class="text-center lg:w-[230px] xl:w-[287px]">
            <div class="relative">
            <img :src="menu.img" alt="">
            <img src="/asset/plays.png" class="absolute top-0 left-0 w-full opacity-0 hover:opacity-100 transition-all duration-300 cursor-pointer" alt="">
            </div>
            <p class="font-medium text-xl text-[#272042] my-3" v-text="menu.nama"></p>
            <p class="font-normal text-[#8B8BA5] mb-3" v-text="menu.chef"></p>
            <img :src="menu.star" alt="" class="mx-auto">
        </div>
    </div>

</div>
</template>

<script>
export default {
    data() {
        return {
            menusehat: [
                {
                    img: '/asset/makanan1.png',
                    nama: 'Salad Kiwi Sugga',
                    chef: 'Amir Samantha',
                    star: '/asset/stars.png'
                },
                {
                    img: '/asset/makanan2.png',
                    nama: 'Avocado Muscle',
                    chef: 'Amir Samantha',
                    star: '/asset/stars.png'
                },
                {
                    img: '/asset/makanan3.png',
                    nama: 'Bayam Red Poppeye',
                    chef: 'Amir Samantha',
                    star: '/asset/stars.png'
                },
                {
                    img: '/asset/makanan4.png',
                    nama: 'Niga Fruity Joss',
                    chef: 'Amir Samantha',
                    star: '/asset/stars.png'
                },
            ]
        }
    },
}
</script>