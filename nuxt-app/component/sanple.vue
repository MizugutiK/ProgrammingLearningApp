<script setup lang="js">
import { ref, defineEmits } from 'vue';

// コンポーネント使用例
// 処理を一つのファイル内で書く必要がなくなる＋処理を使いまわしできる

// イベント定義
const emit = defineEmits(['send-value']);

// テキストに入ったデータ情報を入れる箱
const childvalue = ref('');

// ボタンクリックで起こる処理
// ここではemitでsend-valueイベントを発火している
const sendValueToParent = () => {
    emit('send-value', childvalue.value);
};


</script>

<template>
    <!-- InputTextとButton はPrimeVew -->
    <InputText type="text" v-model="childvalue" />
    <Button @click="sendValueToParent" label="送信" />
</template>