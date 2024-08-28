<script setup>
import ExampleCard from "../Components/ExampleCard.vue";
import MaterialBadge from "../../../components/MaterialBadge.vue";

</script>
<template>

  <section class="py-5">
    <div class="container">
      <div class="row">
        <div class="row text-center my-sm-5 mt-5">
          <div class="col-lg-6 mx-auto">

            <h2>다올피플 소식</h2>
          </div>
        </div>
      </div>
    </div>
    <div class="container mt-5">
      <div class="row">
        <div class="col-md-12">
          <div class="row mt-4">
            <div class="col-md-4 mt-md-0 mt-5">
              <ExampleCard
                class="shadow-lg"
                title="구리 다올피플, 복지취약계층 후원금 인창동 행복센터에 전달"
                image="https://cdn.kihoilbo.co.kr/news/photo/202301/1010913_381897_5350.jpg"
                link="https://www.kihoilbo.co.kr/news/articleView.html?idxno=1010913"
              />
            </div>

            <div class="col-md-4 mt-md-0 mt-5">
              <ExampleCard
                class="shadow-lg"
                title="[2022 광운대 스타트업 CEO] 유통 웹·모바일 시스템 구축하는 스타트업 ‘다올피플’"
                image="https://img.hankyung.com/photo/202209/01.31206095.1.jpg"
                link="https://magazine.hankyung.com/job-joy/article/202209135971d"
              />
            </div>

            <div class="col-md-4 mt-md-0 mt-5">
              <ExampleCard
                class="shadow-lg"
                title="구리시 청년창업 유망 스타트업 ‘쑥쑥’…지원다채"
                image="https://image.fnnews.com/resource/media/image/2021/11/07/202111070523337564_l.jpg"
                link="https://www.fnnews.com/news/202111070518248853"
              />
            </div>

            <div class="col-md-4 mt-md-0 mt-5">
              <ExampleCard
                class="shadow-lg"
                title="구리시 청년창업지원센터 2022년 성과공유회 개최"
                image="https://www.kmaeil.com/news/photo/202211/374612_200337_4318.jpg"
                link="https://www.kmaeil.com/news/articleView.html?idxno=374612"
              />
            </div>


          </div>
        </div>
      </div>
    </div>
  </section>

</template>
