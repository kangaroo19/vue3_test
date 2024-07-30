<script setup>
import { Accessibility } from "accessibility";

var options = {
  labels: {
    resetTitle: "reset (in my language)",
    closeTitle: "close (in my language)",
    menuTitle: "타이틀ㅇ",
    increaseText: "텍스트 크기 증가",
    decreaseText: "decrease text size (in my language)",
    increaseTextSpacing: "increase text spacing (in my language)",
    decreaseTextSpacing: "decrease text spacing (in my language)",
    increaseLineHeight: "increase line height (in my language)",
    decreaseLineHeight: "decrease line height (in my language)",
    invertColors: "invert colors (in my language)",
    grayHues: "gray hues (in my language)",
    underlineLinks: "underline links (in my language)",
    bigCursor: "big cursor (in my language)",
    readingGuide: "reading guide (in my language)",
    textToSpeech: "텍스트를 음성으로",
    speechToText: "음성을 텍스트로",
    disableAnimations: "disable animations (in my language)",
    hotkeyPrefix: "Hotkey: (in my language)",
  },
  hotkeys: {
    enabled: true,
  },
  icon: {
    circular: true,
  },
  language: {
    textToSpeechLang: "en-US",
    speechToTextLang: "en-US",
  },
};
var instance = new Accessibility(options);
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />

  <div>
    <div aria-live="polite">
      This website is designed to provide users with a wealth of information.
      The navigation is simple, allowing access to a wide range of content.
      Furthermore, we regularly update the site to enhance the user experience
      and ensure the information is current and relevant.
    </div>
    <div>
      이 웹사이트는 사용자에게 풍부한 정보를 제공하기 위해 설계되었습니다.
      내비게이션이 간단하여 다양한 콘텐츠에 쉽게 접근할 수 있습니다. 또한,
      사용자 경험을 향상시키고 정보를 최신 상태로 유지하기 위해 정기적으로
      사이트를 업데이트합니다.
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  background: black;
  margin: 0;
  padding: 0;
}
</style>
