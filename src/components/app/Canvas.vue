<template>
  <canvas ref="canvas" class="canvas"></canvas>
</template>

<script lang="ts" setup>
import { onMounted, Ref, ref } from 'vue';

type Props = {
  title: string;
}

const props = defineProps<Props>();
const canvas: Ref<HTMLCanvasElement | null> = ref(null);

onMounted(() => {
  const ctx = canvas.value!.getContext('2d');
  const { width, height } = canvas.value!

  ctx!.font = '30px Arial';
  ctx!.textAlign = 'center';
  ctx!.fillText(props.title, width / 2, height /2)
})
</script>

<style lang="sass" scoped>
.canvas
  display: block
  width: 100%
</style>
