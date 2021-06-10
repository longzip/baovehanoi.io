<template>
  <main>
    <social-head
      :description="'Tìm ngay việc làm bảo vệ tại Hà Nội, đăng ký ứng tuyển, nhận thông báo tuyển dụng việc làm và hỗ trợ trò chuyện miễn phí.'"
      :title="'Việc làm bảo vệ tại Hà Nội'"
      :image="'https://baovehanoi.ga/images/viec-lam-bao-ve-tai-ha-noi.jpg'"
    />
    <header-component />
    <section-top />
    <section-one />
    <section-two />
    <section-three />
    <section-four />
  </main>
</template>
<script>
import SocialHead from '@/components/SocialHead.vue'
import HeaderComponent from '@/components/Header.vue'
import SectionTop from '@/components/SectionTop.vue'
import SectionOne from '@/components/SectionOne.vue'
import SectionTwo from '@/components/SectionTwo.vue'
import SectionThree from '@/components/SectionThree.vue'
import SectionFour from '@/components/SectionFour.vue'
export default {
  components: {
    SocialHead,
    HeaderComponent,
    SectionTop,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
  },
}
</script>
