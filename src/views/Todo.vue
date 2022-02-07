<template>

  <div>
    
    <Me @Input="validate"></Me>
    <Ja :J1="J1"></Ja>
    </div>
    
</template>

<script>
import Me from "../components/Me.vue"
import Ja from "../components/Ja.vue"
export default {
  data: () => ({
    J1: [],
  }),
components :{Me,Ja},
J1: "Input",
  methods: {
    validate(select, name) {
      this.J1.push({
        name: select + " : " + name,
      });
    },
  },
};
</script>

<style>

</style>