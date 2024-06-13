<script>
import HomeCarousel from "../components/HomeCarousel.vue";
import PartnerSection from "../components/PartnerSection.vue";
import HomeSupport from "../components/HomeSupport.vue";
import HomeInfoCard from "../components/HomeInfoCard.vue";
import HomeOurMission from "../components/HomeOurMission.vue";
import HomeStatistics from "../components/HomeStatistics.vue";
import HomePastProjects from "../components/HomePastProjects.vue";
import HomeReviews from "../components/HomeReviews.vue";
import HomeProjectsExamples from "../components/HomeProjectsExamples.vue";
import HomeNews from "../components/HomeNews.vue";

export default {
  name: "Home",

  components: {
    HomeCarousel,
    PartnerSection,
    HomeSupport,
    HomeInfoCard,
    HomeOurMission,
    HomeStatistics,
    HomePastProjects,
    HomeReviews,
    HomeProjectsExamples,
    HomeNews,
  },

};
</script>

<template>
  <!--jumbo-->
  <section>
    <HomeCarousel />
  </section>

  <!--we are-->
  <section>
    <HomeInfoCard />
  </section>

  <!--learn more-->
  <section>
    <HomeOurMission />
  </section>

  <!--past projects-->
  <section>
    <HomePastProjects />
  </section>

  <!--examples-->
  <section>
    <HomeProjectsExamples />
  </section>

  <!--we love-->
  <section>
    <HomeStatistics />
  </section>

  <!--support-->
  <section>
    <HomeSupport />
  </section>

  <!--reviews-->
  <section>
    <HomeReviews />
  </section>

  <!--blog-->
  <section>
    <HomeNews />
  </section>

  <!--partners-->
  <PartnerSection />
</template>

<style scoped lang="scss">

.we-love {
  .col-6:first-of-type {
    background-image: url("https://demo.phlox.pro/business-2/wp-content/uploads/sites/57/2018/08/person-with-long-curly-hair-PZ99QM2@2x.jpg");
  }
}

.reviews {
  background-image: url("https://demo.phlox.pro/business-2/wp-content/uploads/sites/57/2018/08/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg");
}
</style>
