<template>
  <div>
    <page-header />
    <nuxt />
    <migration />
    <page-footer />
  </div>
</template>

<script>
import PageHeader from '~/components/common/PageHeader.vue'
import PageFooter from '~/components/common/PageFooter.vue'
import Migration from '~/components/top/Migration.vue'
export default {
  components: {
    PageHeader,
    Migration,
    PageFooter
  }
}
</script>