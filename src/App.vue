<template>
  <div class="flex justify-center mt-24">
    <div></div>
    <div class="w-2/4">
      <div>
        <p class="text-3xl mb-5 text-center">国际音标表</p>

        <hr />

        <p class="text-xl mb-5 p-3">
          48个国际音标通常是国内学生学习英语、学好英语发音必须掌握的发音基础，48个国际音标表也被称作48个音标表、48个英语音标表、48个英语国际英标表，48个国际英语音标表，这些称呼通常都是指48个英语国际英标表。48个国际音标中有20个元音、28个辅音，为了便于同学们学习和记忆巴士英语网为大家整理了这些音标表，希望能帮助到大家!
        </p>
      </div>
      <table
        class="
          mt-5
          table-auto
          border-separate border border-green-800
          font-serif
        "
      >
        <thead>
          <tr>
            <th class="border border-green-600">Title</th>
            <th class="border border-green-600">Author</th>
            <th class="border border-green-600">Views</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td class="border border-green-600" @mousemove="playAudio('01')">
              Chris
            </td>
            <td class="border border-green-600" @mousemove="playAudio('02')">
              Chris
            </td>
            <td class="border border-green-600" @mousemove="playAudio('03')">
              Chris
            </td>
            <td class="border border-green-600" @mousemove="playAudio('04')">
              Chris
            </td>
            <td class="border border-green-600" @mousemove="playAudio('05')">
              Chris
            </td>
            <td class="border border-green-600" @mousemove="playAudio('06')">
              Chris
            </td>
            <td class="border border-green-600" @mousemove="playAudio('07')">
              Chris
            </td>
          </tr>
        </tbody>
      </table>
    </div>
    <div></div>
  </div>
</template>

<script>
import _ from "lodash";

export default {
  name: "App",
  methods: {
    // playAudio(num) {
    //   console.log(num);
    //   var audio = new Audio(require(`./assets/mp3s/02.mp3`)); // path to file
    //   audio.play();
    //   // this.d()
    //   _.debounce(() => {}, 550);
    // },
    playAudio: _.debounce(() => {
      if (audio) {
        audio.ended()
      }
      var audio = new Audio(require(`./assets/mp3s/02.mp3`)); // path to file
      audio.play();
    }, 200),
    d() {},
  },
};
</script>

<style>
body {
  background: rgb(65, 65, 65);
}

body p {
  color: white;
}
</style>
