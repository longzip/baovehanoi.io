<template>
  <div
    class="relative pt-16 pb-32 flex content-center items-center justify-center"
    style="min-height: 75vh"
  >
    <div
      class="absolute top-0 w-full h-full bg-center bg-cover"
      :style="`background-image: url('${imageUrl}')`"
    >
      <span
        id="blackOverlay"
        class="w-full h-full absolute opacity-75 bg-black"
      ></span>
    </div>
    <div class="container relative mx-auto">
      <div class="items-center flex flex-wrap">
        <div class="w-full lg:w-6/12 px-4 ml-auto mr-auto text-center">
          <div class="pr-12">
            <h1 class="text-white font-semibold text-5xl">
              {{ title }}
            </h1>
            <p v-if="shortDescription" class="mt-4 text-lg text-gray-300">
              {{ shortDescription }}
            </p>
          </div>
        </div>
      </div>
    </div>
    <div
      class="
        top-auto
        bottom-0
        left-0
        right-0
        w-full
        absolute
        pointer-events-none
        overflow-hidden
      "
      style="height: 70px"
    >
      <svg
        class="absolute bottom-0 overflow-hidden"
        xmlns="http://www.w3.org/2000/svg"
        preserveAspectRatio="none"
        version="1.1"
        viewBox="0 0 2560 100"
        x="0"
        y="0"
      >
        <polygon
          class="text-gray-300 fill-current"
          points="2560 0 2560 100 0 100"
        ></polygon>
      </svg>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    imageUrl: {
      type: String,
      default: '/images/viec-lam-bao-ve-tai-ha-noi.jpg',
    },
    title: {
      type: String,
      default: 'Việc làm bảo vệ tại Hà Nội',
    },
    shortDescription: {
      type: String,
      default:
        'Nhân viên bảo vệ là người sẽ ngăn chặn việc xấu xảy ra với con người hay tài sản. Họ là người sẽ trực tiếp đi tuần tra, chống trộm cắp, phá hoại và ngăn chặn các hoạt động diễn ra bất hợp pháp. Nhân viên bảo vệ hiện có mặt ở tất cả mọi nơi từ trường học, bệnh viện.. cho đến nhà hàng, cao ốc.',
    },
  },
}
</script>
