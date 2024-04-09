<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar class="q-py-md bg-skyblue text-white">
        <!-- left :: start -->
        <div class="text-h5">
          Hyperhire
        </div>
        <!-- left :: end -->
        <q-space></q-space>
        <!-- middle :: start -->
        <div>
          <!-- dropdownBtn :: start -->
          <q-btn-dropdown stretch flat label="채용">
            <q-list>
              <q-item-label header>Folders</q-item-label>
              <q-item v-for="n in 3" :key="`x.${n}`" clickable v-close-popup tabindex="0">
                <q-item-section avatar>
                  <q-avatar icon="folder" color="secondary" text-color="white" />
                </q-item-section>
                <q-item-section>
                  <q-item-label>Photos</q-item-label>
                  <q-item-label caption>February 22, 2016</q-item-label>
                </q-item-section>
                <q-item-section side>
                  <q-icon name="info" />
                </q-item-section>
              </q-item>
              <q-separator inset spaced />
              <q-item-label header>Files</q-item-label>
              <q-item v-for="n in 3" :key="`y.${n}`" clickable v-close-popup tabindex="0">
                <q-item-section avatar>
                  <q-avatar icon="assignment" color="primary" text-color="white" />
                </q-item-section>
                <q-item-section>
                  <q-item-label>Vacation</q-item-label>
                  <q-item-label caption>February 22, 2016</q-item-label>
                </q-item-section>
                <q-item-section side>
                  <q-icon name="info" />
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
          <!-- dropdownBtn :: end -->

          <q-btn stretch flat label="해외 개발자 활용 서비스" />
        </div>
        <!-- middle :: end -->
        <q-space></q-space>
        <!-- right :: start -->
        <div>
          <q-btn color="info" outline class="bg-white text-dark">문의하기</q-btn>
        </div>
        <!-- right :: end -->
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup lang="ts">
// import { ref } from 'vue';

</script>
