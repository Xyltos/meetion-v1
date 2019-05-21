<template>
  <q-layout view="lHh Lpr lFf">
    <q-layout-drawer side="right"
                     v-model="showRight"
                     content-class="bg-grey-3"
                     no-hide-on-route-change=true>
      <div id="test">
        {{time}}
      </div>
    </q-layout-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { openURL } from 'quasar';

export default {
  name: 'LayoutDefault',
  data() {
    return {
      time: 'tijd hier aaaaaaaa',
    }
  },
  computed: {

  },
  methods: {
    openURL,
  },
};
</script>

<style>
</style>
