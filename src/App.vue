<template>
  <!-- <VApp></VApp> -->
  <!-- 網站主體用 v-app -->
  <v-app>
    <!-- 導覽列用 v-app-bar -->
    <v-app-bar>
      <!-- 導覽列標題用 v-app-bar-title -->
      <v-app-bar-title>校園社團介紹網</v-app-bar-title>
      <!-- 要加 mdi 在前面 -->
      <!-- active="false" 文字-->
      <!-- :active="false" 布林值 -->
      <v-btn prepend-icon="mdi-home" to="/" :active="false">回首頁</v-btn>
      <!-- 如果不加:active="false"會一直亮 -->
    </v-app-bar>
    <!-- 網站內容用 v-main -->
    <v-main>
      <!-- 顯示路由元件 -->
      <router-view></router-view>
    </v-main>
    <!-- footer 用 v-footer，加上 app 可以固定在底部 -->
    <v-footer app>
      最近更新日期：2023/03/30
    </v-footer>
  </v-app>
</template>
