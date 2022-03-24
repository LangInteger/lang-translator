<template>
  <div class="cst-result" :data-cst-theme="theme" :data-cst-status="result.status" v-if="result">
    <h6 class="cst-result-text" v-if="result.text">{{ result.text }}</h6>
    <div style="margin-top:5px ;">
        <button v-on:click="playEn()">英 📣</button>
        <button v-on:click="playUs()">美 📢</button>
    </div>
    <pre class="cst-result-phonetic" v-if="result.phonetic">{{ result.phonetic }}</pre>
    <div class="cst-result-translation" v-html="result.translation"></div>

    <audio id="enAudio" controls="controls">
        <source :src="enAudioLink" type="audio/mpeg">
    </audio>
    <audio id="usAudio" controls="controls">
        <source :src="usAudioLink" type="audio/mpeg">
    </audio>

  </div>
</template>

<script>
export default {
  props: ['result', 'theme'],
  data: function() {
    return {
      enAudioLink: 'https://dict.youdao.com/dictvoice?type=1&audio=' + this.result.text,
      usAudioLink: 'https://dict.youdao.com/dictvoice?type=0&audio=' + this.result.text
    }
  },
  methods: {
    playEn(event) {
      var myAudio = document.getElementById("enAudio");
      myAudio.play();
    },
    playUs(event) {
      var myAudio = document.getElementById("usAudio");
      myAudio.play();
    },
  },
}
</script>
