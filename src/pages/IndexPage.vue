<template>
  <!-- firstRow :: start -->
  <div class="maruthi">
    <div class="row justify-between q-py-lg">
      <div class="col-12 col-md-6">
        <div class="q-pa-lg">
          <div class="q-ma-sm">
            <div class="q-mb-md">
              <q-btn color="secondary">풀타임, 파트타임</q-btn>
            </div>
            <div class="text-h5">최고의 실력을 가진
              외국인 인재를 찾고 계신가요?</div>
            <div class="text-caption q-my-md">
              법률 및 인사관리 부담없이
              1주일 이내에 원격으로 채용해보세요.
            </div>
            <div class="text-caption">
              개발자가 필요하신가요?
            </div>
            <br />

            <a href="#">
              개발자가 필요하신가요?
            </a>
          </div>
          <div class="row q-my-lg">
            <div class="col-12 col-md-4" v-for="item, index in 3" :key="index">
              <div class="q-pa-sm">
                <div style="border-top: 1px solid grey">
                  <div class="text-h6 q-py-md">평균 월 120만원</div>
                  <div class="text-caption">
                    임금을 해당 국가를 기준으로 계산합니다.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6">
        <div class="q-pa-lg">
         <SwiperComp />
        </div>
      </div>
      <div class="col-12 col-md-3" v-for="n in 4" :key="n">

        <div style="border: 1px solid grey; border-radius: 0.5rem;" class="q-pa-md q-ma-md">

          <div class="row items-center">
            <div class="q-mr-md">
              <q-btn outline icon="home"></q-btn>
            </div>
            <div>
              해외 마케팅
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>
  <!-- firstRow :: end -->

  <div class="q-mt-xl">
    <!-- secondRow :: start -->
    <div class="row items-center">
      <div class="col-12 col-md-4">
        <div class="row">
          <div class="col-12">
            <div class="q-ma-md q-pa-md">
              <div class="text-h6">Hyperhire</div>
              <div class="text-caption q-my-md">
                우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.
              </div>
              <div class="text-caption text-bold">
                010-0000-0000
              </div>
              <div class="text-caption text-bold">
                aaaaa@naver.com
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-8">
        <div class="row items-center">
          <div class="col-12 col-md-3" v-for="l in 4" :key="l">
            <div class="q-ma-md">
              <q-card class="q-pa-md" style="border-radius: 0.5rem;">
                <div>
                  <q-btn dense icon="home" size="sm" class="q-px-sm"></q-btn>
                </div>
                <div class="text-caption q-my-md">
                  해외 개발자 원격 채용
                </div>
                <div class="row justify-start items-center">
                  <div class="text-caption q-mr-xs">
                    바로가기
                  </div>
                  <div>
                    <q-btn icon="arrow_forward" size="0.3rem" outline class="q-px-xs"></q-btn>
                  </div>
                </div>
              </q-card>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- secondRow :: start -->

    <!-- thirdRow :: start -->
    <div class="row">
      <div class="col-12 col-md-3" v-for="j in 4" :key="j">
        <div class="q-ma-md">
          <div class="q-pa-lg">
            <div class="text-title text-bold">상호명</div>
            <div class="text-caption">하이퍼하이어</div>
            <div class="text-caption">Hyperhire India Private Limited</div>
          </div>
        </div>
      </div>
    </div>
    <!-- thirdRow :: start -->

    <!-- footer :: start -->
    <div class="row justify-start">
      <div class="col-12 q-pa-lg">
        @2024 - Hyperhire
      </div>
    </div>
    <!-- footer :: end -->
  </div>
</template>

<script setup lang="ts">
import { onMounted } from 'vue';
import Swiper from 'swiper'
import 'swiper/swiper-bundle.css';
import SwiperComp from 'src/components/SwiperComp.vue';

onMounted(() => {
  // eslint-disable-next-line @typescript-eslint/no-unused-vars
  const mySwiper = new Swiper('.swiper-container', {
    // Swiper options here...
  });
})
</script>

<style lang="scss" scoped>
/* Add any other custom styles here */
.maruthi {
  background: linear-gradient(to top left, skyblue, transparent);
}

/* Adjust height of swiper-container to fit the content */
.swiper-container {
  overflow: hidden;
}

/* Adjust width of swiper-slide to fit the container */
.swiper-slide {
  width: 100%;
}

</style>