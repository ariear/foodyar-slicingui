<template>
  <footer class="border-t flex justify-evenly flex-wrap py-10 font-pupylinux">
      <div>
          <p class="font-normal text-[28px] hidden md:block">🍔 Foodyar</p>
      </div>
      <div v-for="(content, index) in contentfooter" :key="index" class="mt-5">
          <p class="font-medium text-[#272042] text-[19px] md:text-[22px]" v-text="content.title"></p>
          <p class="font-light text-[#8B8BA5] mt-2 text-sm md:text-base" v-for="(cintil, index) in content.content" :key="index" v-text="cintil.text"></p>
      </div>
  </footer>
  <footer class="border-t text-center font-pupylinux py-7">
      <p class="font-light text-[#8B8BA5]">Foodyar Slicing By Arie</p>
  </footer>
</template>

<script>
export default {
    data() {
        return {
            contentfooter: [
                {
                    'title' : 'Special Course',
                    'content': [
                        {
                            'text': 'Wedding Foods'
                        },
                        {
                            'text': 'Healthy and Muscle'
                        },
                        {
                            'text': 'Office Food Daily'
                        },
                        {
                            'text': 'Happy Kids'
                        },
                    ]
                },
                {
                    'title' : 'Company',
                    'content': [
                        {
                            'text': 'APIs Developer'
                        },
                        {
                            'text': 'Career'
                        },
                        {
                            'text': 'Terms & Conditions'
                        },
                        {
                            'text': 'Privacy Policy'
                        },
                    ]
                },
                {
                    'title' : 'Be Our Friend',
                    'content': [
                        {
                            'text': '3, Season Park, Jakarta'
                        },
                        {
                            'text': 'support@foodyar.co,id'
                        },
                        {
                            'text': '021 - 1111 - 2222'
                        }
                    ]
                },
            ]
        }
    },
}
</script>