<script lang="ts">
  import { Button } from "$lib/components/ui/button"
  import { Star } from 'lucide-svelte'
  let count: number = 0
  const increment = () => {
    count += 1
  }
</script>

<div class="w-screen h-screen flex flex-col justify-center items-center gap-4">
  <Star color="#FB923C" size={512} strokeWidth={1} class="absolute opacity-10 animate-slow-spin z-0" />
  <div class="flex justify-center items-center gap-4 z-10">
    <Button class="w-32 h-min bg-orange-500 hover:bg-orange-400 text-xl" on:click={increment} >Count is {count}</Button>
    <div class="flex flex-col justify-center items-start">
      <h1 class="font-bold text-2xl text-orange-500">QuickSvelte Template</h1>
      <p class="italic">Svelte + TypeScript + shadcn/ui + Lucide</p>
      <a target="_blank" class="underline" href="https://github.com/skittlexyz/">github.com/skittlexyz</a>
    </div>
  </div>
</div>