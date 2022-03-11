<template>
  <div class="font-pupylinux md:w-[700px] lg:w-[790px] mx-auto pt-0 md:pt-16">
      <p class="font-light text-xl md:text-4xl text-[#272042] text-center px-4 md:px-0" v-text="testi"></p>
      <div class="flex items-center justify-center mt-10">
          <img src="/asset/pptesti.png" class="rounded-full w-[60px]" alt="">
          <div class="ml-6">
              <p class="font-medium text-xl">Camella Sarrah</p>
              <p class="font-light text-[#8B8BA5]">Vege Master</p>
          </div>
      </div>
  </div>
  <div class="container mx-auto flex flex-wrap justify-evenly text-center mt-20 pb-20">
      <div v-for="(data, index) in datafek" :key="index" class="mt-5 md:mt-0">
          <p class="font-bold text-[#272042] text-3xl" v-text="data.jml"></p>
          <p class="font-light text-[#8B8BA5] text-lg" v-text="data.ket"></p>
      </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            testi: 'Awalnya saya malu dengan mertua karena tidak bisa memasak, kini mereka lebih suka makan malam di rumah demi menyantap masakan yang saya buat sendiri',
            datafek: [
                {
                    jml: '180.000+',
                    ket: 'MENU FOOD'
                },
                {
                    jml: '20.000+',
                    ket: 'CHEFS'
                },
                {
                    jml: '180.000+',
                    ket: 'COURSE'
                },
                {
                    jml: '6.900.000',
                    ket: 'ALUMNI'
                },
            ]
        }
    },
}
</script>