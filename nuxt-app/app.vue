<script setup lang="js">
import { ref } from 'vue';

//これを書かないとコンポーネントは動かない 
// 書かなくて動くのはPrimeVewに入っているものだけ
import sanple from './component/sanple.vue';

// sanpule.vueからデータが送られるとここの値が変化する
const parentValue = ref('デフォ');
</script>

<template>
  <div>
    テスト
    <!-- Primevue -->
    <Button label="Check" />
    <Button label="Submit" />
    <!-- PrimeFlex -->
    <div class="surface-500 font-bold border-round m-2 flex align-items-center justify-content-center"
      style="min-width: 200px; min-height: 100px">
      surface-500
    </div>
    <div class="block bg-primary font-bold text-center p-4 border-round mb-3">3</div>
  </div>

  <!-- コンポーネント例 -->

  <!-- parentValue には初期の値”デフォ”が入る -->
  <p>親コンポーネントの値: {{ parentValue }}</p>

  <!-- sanlpe.vueをコンポーネントとして使用している -->
  <!-- sendValueイベントを受け取れるようにし、受け取った値をparentValueに格納 -->
  <sanple @send-value="parentValue = $event" />

</template>
