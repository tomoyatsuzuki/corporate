<template>
  <div>
    <div class='container'><page-header />
      <hero />
      <mission />
      <results :items="results.items"/>
      <features />
      <bussiness />
      <menber />
      <update />
      <company />
    </div>
  </div>
</template>


<script>
import PageHeader from '~/components/common/PageHeader.vue'
import Hero from '~/components/top/Hero.vue'
import Mission from '~/components/top/Mission.vue'
import Results from '~/components/top/Results.vue'
import Features from '~/components/top/Features.vue'
import Bussiness from '~/components/top/Bussiness.vue'
import Member from '~/components/top/Member.vue'
import Update from '~/components/top/Update.vue'
import Company from '~/components/top/Company.vue'
import Migration from '~/components/top/Migration.vue'
import PageFooter from '~/components/common/PageFooter.vue'

export default {
  components: {
    Hero,
    Mission,
    Results,
    Features,
    Bussiness,
    Member,
    Update,
    Company,
  },
  data() {
    return {
      results: {
        items: [
          {
        url: 'https://www.kikagaku.co.jp' ,
        img_url: require('~/assets/img/front/portfolio/image1.jpg'),
        img_alt: 'Preferred Networks社提供のChainerチュートリアル制作に協力',
        title: 'Preferred Networks社提供のChainerチュートリアル制作に協力',
          },
      {
      url: 'https://www.kikagaku.co.jp' ,
        img_url: require("~/assets/img/front/portfolio/image2.jpg"),
        img_alt: 'メルカリ社の経営層向けAI研修の実施',
        title: 'メルカリ社の経営層向けAI研修の実施aa',
      },
          {
      url: 'https://www.kikagaku.co.jp' ,
        img_url: require('~/assets/img/front/portfolio/image3.jpg'),
        img_alt: 'ABEJA社とアセスメント人材育成コースを共同制作',
        title: 'ABEJA社とアセスメント人材育成コースを共同制作',
          }
        ]
     }
    }
  }
}
</script>