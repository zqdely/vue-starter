<template>
  <div :class="$style.form">
    <vue-grid>
      <vue-breadcrumb :items="[{ label: 'Home', href: '/' }, { label: 'Form Example' }]" />

      <vue-grid-row>
        <vue-grid-item class="vueGridItem">
          <vue-headline level="1">Form example</vue-headline>
          <form-example />
        </vue-grid-item>

        <vue-grid-item class="vueGridItem"></vue-grid-item>
      </vue-grid-row>
    </vue-grid>
  </div>
</template>

<script lang="ts">
import VueGrid from '../../shared/components/VueGrid/VueGrid.vue';
import VueGridRow from '../../shared/components/VueGridRow/VueGridRow.vue';
import VueGridItem from '../../shared/components/VueGridItem/VueGridItem.vue';
import FormExample from '../FormExample/FormExample.vue';
import VueHeadline from '../../shared/components/VueHeadline/VueHeadline.vue';
import VueBreadcrumb from '../../shared/components/VueBreadcrumb/VueBreadcrumb.vue';

export default {
  metaInfo: {
    title: 'vue-starter - Form Example',
  },
  components: { VueBreadcrumb, VueHeadline, FormExample, VueGridItem, VueGridRow, VueGrid },
  computed: {},
  data(): any {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" module>
@import '~@/app/shared/design-system';

.form {
  padding-top: $nav-bar-height;
  padding-bottom: $space-unit * 2;
}
</style>
