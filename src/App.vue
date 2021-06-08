<template>
  <div class="flex justify-center mt-24">
    <div></div>
    <div class="w-10/12 lg:w-3/5">
      <div>
        <p class="text-3xl mb-5 text-center">国x际音标表</p>

        <hr />

        <p class="text-xl mb-5 p-3">
          48个国际音标中有20个元音、28个辅音，为了便于同学们学习和记忆巴士英语网为大家整理了这些音标表，希望能帮助到大家!
        </p>
      </div>

      <div class="grid grid-cols-8 gap-2 w-full text-center my-5">
        <div class="bg-gray-400 flex justify-center items-center row-span-5">
          元音
        </div>
        <div class="bg-gray-400 flex justify-center items-center row-span-3">
          单元音
        </div>
        <div class="bg-gray-400">前元音</div>
        <div class="bg-gray-400" @click="playAudio('iː')">/iː/</div>
        <div class="bg-gray-400" @click="playAudio('ɪ')">/ɪ/</div>
        <div class="bg-gray-400" @click="playAudio('e')">/e/</div>
        <div class="bg-gray-400" @click="playAudio('æ')">/æ/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">中元音</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400" @click="playAudio('ɜː')">/ɜː/</div>
        <div class="bg-gray-400" @click="playAudio('ə')">/ə/</div>
        <div class="bg-gray-400" @click="playAudio('ʌ')">/ʌ/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">后元音</div>
        <div class="bg-gray-400" @click="playAudio('uː')">/uː/</div>
        <div class="bg-gray-400" @click="playAudio('ʊ')">/ʊ/</div>
        <div class="bg-gray-400" @click="playAudio('ɔː')">/ɔː/</div>
        <div class="bg-gray-400" @click="playAudio('ɒ')">/ɒ/</div>
        <div class="bg-gray-400" @click="playAudio('ɑː')">/ɑː/</div>
        <div class="bg-gray-400 flex justify-center items-center row-span-2">
          双元音
        </div>
        <div class="bg-gray-400">开合双元音</div>
        <div class="bg-gray-400" @click="playAudio('eɪ')">/eɪ/</div>
        <div class="bg-gray-400" @click="playAudio('aɪ')">/aɪ/</div>
        <div class="bg-gray-400" @click="playAudio('ɔɪ')">/ɔɪ/</div>
        <div class="bg-gray-400" @click="playAudio('aʊ')">/aʊ/</div>
        <div class="bg-gray-400" @click="playAudio('əʊ')">/əʊ/</div>
        <div class="bg-gray-400">集中双元音</div>
        <div class="bg-gray-400" @click="playAudio('ɪə')">/ɪə/</div>
        <div class="bg-gray-400" @click="playAudio('eə')">/eə/</div>
        <div class="bg-gray-400" @click="playAudio('ʊə')">/ʊə/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div
          class="bg-gray-400 flex justify-center items-center"
          style="grid-row: span 9 / span 9"
        >
          辅音
        </div>
        <div class="bg-gray-400 flex justify-center items-center row-span-2">
          爆破音
        </div>
        <div class="bg-gray-400">清辅音</div>
        <div class="bg-gray-400" @click="playAudio('p')">/p/</div>
        <div class="bg-gray-400" @click="playAudio('t')">/t/</div>
        <div class="bg-gray-400" @click="playAudio('k')">/k/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">浊辅音</div>
        <div class="bg-gray-400" @click="playAudio('b')">/b/</div>
        <div class="bg-gray-400" @click="playAudio('d')">/d/</div>
        <div class="bg-gray-400" @click="playAudio('g')">/ɡ/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400 flex justify-center items-center row-span-2">
          摩擦音
        </div>
        <div class="bg-gray-400">清辅音</div>
        <div class="bg-gray-400" @click="playAudio('f')">/f/</div>
        <div class="bg-gray-400" @click="playAudio('s')">/s/</div>
        <div class="bg-gray-400" @click="playAudio('ʃ')">/ʃ/</div>
        <div class="bg-gray-400" @click="playAudio('θ')">/θ/</div>
        <div class="bg-gray-400" @click="playAudio('h')">/h/</div>
        <div class="bg-gray-400">浊辅音</div>
        <div class="bg-gray-400" @click="playAudio('v')">/v/</div>
        <div class="bg-gray-400" @click="playAudio('z')">/z/</div>
        <div class="bg-gray-400" @click="playAudio('ʒ')">/ʒ/</div>
        <div class="bg-gray-400" @click="playAudio('ð')">/ð/</div>
        <div class="bg-gray-400" @click="playAudio('r')">/r/</div>
        <div class="bg-gray-400 flex justify-center items-center row-span-2">
          破擦音
        </div>
        <div class="bg-gray-400">清辅音</div>
        <div class="bg-gray-400" @click="playAudio('tʃ')">/tʃ/</div>
        <div class="bg-gray-400" @click="playAudio('tr')">/tr/</div>
        <div class="bg-gray-400" @click="playAudio('ts')">/ts/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">浊辅音</div>
        <div class="bg-gray-400" @click="playAudio('dʒ')">/dʒ/</div>
        <div class="bg-gray-400" @click="playAudio('dr')">/dr/</div>
        <div class="bg-gray-400" @click="playAudio('dz')">/dz/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">鼻音</div>
        <div class="bg-gray-400">（浊辅音）</div>
        <div class="bg-gray-400" @click="playAudio('m')">/m/</div>
        <div class="bg-gray-400" @click="playAudio('n')">/n/</div>
        <div class="bg-gray-400" @click="playAudio('ŋ')">/ŋ/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">舌则音</div>
        <div class="bg-gray-400">（浊辅音）</div>
        <div class="bg-gray-400" @click="playAudio('l')">/l/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400">半元音</div>
        <div class="bg-gray-400">（浊辅音）</div>
        <div class="bg-gray-400" @click="playAudio('j')">/j/</div>
        <div class="bg-gray-400" @click="playAudio('w')">/w/</div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
        <div class="bg-gray-400"></div>
      </div>

      <footer class="text-white">
        <ul class="list-disc">
          <li>
            音频来源：https://www.bilibili.com/video/BV1Y4411M7Ac?from=search&seid=12717483388753801542
          </li>
        </ul>
      </footer>
    </div>
    <div></div>
  </div>
</template>

<script>
import { dic } from "./phonetic-symbol-number-dic";

export default {
  name: "App",
  methods: {
    playAudio (ps) {
      var audio = new Audio(require(`./assets/mp3s/${dic[ps]}.mp3`)); // path to file
      audio.play();
    },
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