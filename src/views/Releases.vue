<template>
  <div id="releases">
    <div class="releases-table-wrapper">
      <h1>{{ t('releases.name') }}</h1>
      <div class="generic-page release-table">
        <p>{{ t('releases.version') }} 1.0</p>
        <div>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Reader') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Bootloader') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Recovery') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.SecondDegree') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Trash') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Wallpapers') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Theme') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Parameters') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.SumAndSequences') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Equal') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.NestedRadicals') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Ulab') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.FStrings') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Operators') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Kandinsky') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.ShiftOk') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.FunctionColor') }}</ReleaseItem>
          <ReleaseItem changeType="new">{{ t('releases.versions.1-0.Other') }}</ReleaseItem>
          <ReleaseItem changeType="chg">{{ t('releases.versions.1-0.Scripts') }}</ReleaseItem>
          <ReleaseItem changeType="chg">{{ t('releases.versions.1-0.Storage') }}</ReleaseItem>
          <ReleaseItem changeType="chg">{{ t('releases.versions.1-0.Heap') }}</ReleaseItem>
          <ReleaseItem changeType="chg">{{ t('releases.versions.1-0.Battery') }}</ReleaseItem>
          <ReleaseItem changeType="chg">{{ t('releases.versions.1-0.Apps') }}</ReleaseItem>
          <ReleaseItem changeType="fix">{{ t('releases.versions.1-0.RPN') }}</ReleaseItem>
          <ReleaseItem changeType="fix">{{ t('releases.versions.1-0.Atomic') }}</ReleaseItem>
          <ReleaseItem changeType="fix">{{ t('releases.versions.1-0.Gutter') }}</ReleaseItem>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { useI18n } from 'vue-i18n'
import ReleaseItem from '@/components/ReleaseItem.vue'
export default {
  name: 'ReleasesPage',
  components: {
    ReleaseItem
  },
  setup () {
    const { t } = useI18n({
      inheritLocale: true,
      useScope: 'global'
    })
    return { t }
  }
}
</script>

<style scoped>

#releases {
  display: flex;
  justify-content: center;
}
.releases-table-wrapper {
  max-width: 1000px;
  flex: 1;
}
.release-table{
  padding:2em;
}
</style>
