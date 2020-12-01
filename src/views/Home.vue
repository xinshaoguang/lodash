<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
  mounted() {
    console.dir(_, "_");
    var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 23];
    var a = _.chunk(arr, 3);
    console.log(a, "a");
    // s
    var obj = {
      name: "liudehua",
      age: {
        age: 58,
      },
    };
    var obj1 = _.cloneDeep(obj);
    obj.age.age = 60;
    console.log(obj, obj1);
  },
};
</script>
