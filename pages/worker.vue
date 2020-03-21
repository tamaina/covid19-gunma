<template>
  <div class="Worker">
    <h2 class="Worker-Heading">
      {{ $t('企業の皆様・はたらく皆様へ') }}
    </h2>
    <!-- 
    <StaticCard>
      <h3>
        <a
          href="http://www.sangyo-rodo.metro.tokyo.jp/chushou/kinyu/yuushi/yuushi/new"
          target="_blank"
          rel="noopener"
          >{{ $t('新型コロナウイルス感染症に対応した制度融資') }}</a
        >
      </h3>
      <p>
        {{
          $t(
            '感染症により事業活動に影響を受けている中小企業等を対象とした制度融資（「緊急融資」、「緊急借換」、「危機対応融資」）です。いずれも融資限度額は2億8千万円で、信用保証料を都が補助します。'
          )
        }}
      </p>
    </StaticCard> -->
    <StaticCard />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { MetaInfo } from 'vue-meta'
import StaticCard from '@/components/StaticCard.vue'

type ItemData = {
  items: Item[]
}

type Item = {
  title: string
  link: string
  body: string
}

export default Vue.extend({
  components: {
    StaticCard
  },
  head(): MetaInfo {
    return {
      title: this.$t('企業の皆様・はたらく皆様へ') as string
    }
  }
})
</script>

<style lang="scss">
.Worker {
  &-Heading {
    @include font-size(30);
    font-weight: normal;
    color: $gray-2;
    margin-bottom: 12px;
  }
}
</style>
