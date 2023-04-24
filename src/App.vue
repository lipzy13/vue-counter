<script>
export default {
  components: { Number, ButtonAdd, ButtonMin, Bot},
  data() {
    return {
      num: 0,
    };
  },
  methods: {
      decrease () {
          this.num > 0 ? this.num-- : alert("Can't be less than 0");
          },
      increase () {
          this.num++;
      },
  },
};
import Number from "./components/Number.vue";
import ButtonAdd from "./components/ButtonAdd.vue";
import ButtonMin from "./components/ButtonMin.vue";
import Bot from "./components/Bot.vue";
</script>

<template>
  <div class="w-auto h-screen" id="screnn">
    <div class="flex flex-col items-center justify-center h-full ">
      <Number :num="num" />
      <div class="flex items-center justify-center space-x-4 mt-3">
        <ButtonMin @click = "decrease" />
        <ButtonAdd @click = "increase" />
      </div>
      <Bot />    
    </div>
  </div>
</template>

<style scoped>
#screnn {
  background-color: rgb(250, 232, 255);
        background-image: radial-gradient(at 19% 40%, rgb(251, 146, 60) 0, transparent 43%), radial-gradient(at 10% 2%, rgb(217, 249, 157) 0, transparent 84%), radial-gradient(at 80% 5%, rgb(125, 211, 252) 0, transparent 41%), radial-gradient(at 78% 85%, rgb(224, 231, 255) 0, transparent 21%), radial-gradient(at 60% 73%, rgb(21, 94, 117) 0, transparent 67%), radial-gradient(at 45% 36%, rgb(6, 182, 212) 0, transparent 3%);
}
</style>
