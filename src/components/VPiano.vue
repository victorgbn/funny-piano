<template>
<div>
  <div class="container-piano">
    <div class="key-white" id="key-do"></div>
    <div class="key-white" id="key-re"></div>
    <div class="key-white" id="key-mi"></div>
    <div class="key-white" id="key-fa"></div>
    <div class="key-white" id="key-sol"></div>
    <div class="key-white" id="key-la"></div>
    <div class="key-white" id="key-si"></div>

    <div class="container-key-black">
      <div class="key-black" id="key-do-d"></div>
      <div class="key-black" id="key-re-d"></div>
      <div class="key-black" id="key-fa-d"></div>
      <div class="key-black" id="key-sol-d"></div>
      <div class="key-black" id="key-la-d"></div>
    </div>
  </div>

  <div class="container-note">
    <p>DO</p>
    <p>RÉ</p>
    <p>MI</p>
    <p>FA</p>
    <p>SOL</p>
    <p>LA</p>
    <p>SI</p>
  </div>
</div>
</template>

<script>
export default {
  name: "VPiano",
  mounted() {
    const keyDo = document.getElementById("key-do");
    keyDo.addEventListener("click", () => {
      const noteC = document.createElement("audio");
      noteC.src = "/assets/sounds/C.mp3";
      noteC.play();
    });

    document.addEventListener("keydown", () => {
      if (event.isComposing || event.keyCode === 81) {
        const noteC = document.createElement("audio");
        noteC.src = "/assets/sounds/C.mp3";
        noteC.play();
      }
      if (event.isComposing || event.keyCode === 83) {
        const noteD = document.createElement("audio");
        noteD.src = "/assets/sounds/D.mp3";
        noteD.play();
      }
      if (event.isComposing || event.keyCode === 68) {
        const noteE = document.createElement("audio");
        noteE.src = "/assets/sounds/E.mp3";
        noteE.play();
      }
      if (event.isComposing || event.keyCode === 70) {
        const noteF = document.createElement("audio");
        noteF.src = "/assets/sounds/F.mp3";
        noteF.play();
      }
      if (event.isComposing || event.keyCode === 71) {
        const noteG = document.createElement("audio");
        noteG.src = "/assets/sounds/G.mp3";
        noteG.play();
      }
      if (event.isComposing || event.keyCode === 72) {
        const noteA = document.createElement("audio");
        noteA.src = "/assets/sounds/A.mp3";
        noteA.play();
      }
      if (event.isComposing || event.keyCode === 74) {
        const noteB = document.createElement("audio");
        noteB.src = "/assets/sounds/B.mp3";
        noteB.play();
      }
      if (event.isComposing || event.keyCode === 90) {
        const noteDoD = document.createElement("audio");
        const uriDoD = encodeURIComponent("/assets/sounds/C#.mp3");
        noteDoD.src = uriDoD;
        noteDoD.play();
      }
      if (event.isComposing || event.keyCode === 69) {
        const noteReD = document.createElement("audio");
        const uriReD = encodeURIComponent("/assets/sounds/D#.mp3");
        noteReD.src = uriReD;
        noteReD.play();
      }
      if (event.isComposing || event.keyCode === 84) {
        const noteFaD = document.createElement("audio");
        const uriFaD = encodeURIComponent("/assets/sounds/F#.mp3");
        noteFaD.src = uriFaD;
        noteFaD.play();
      }
      if (event.isComposing || event.keyCode === 89) {
        const noteSolD = document.createElement("audio");
        const uriSolD = encodeURIComponent("/assets/sounds/G#.mp3");
        noteSolD.src = uriSolD;
        noteSolD.play();
      }
      if (event.isComposing || event.keyCode === 85) {
        const noteLaD = document.createElement("audio");
        const uriLaD = encodeURIComponent("/assets/sounds/A#.mp3");
        noteLaD.src = uriLaD;
        noteLaD.play();
      }
    });

    const keyRe = document.getElementById("key-re");
    keyRe.addEventListener("click", () => {
      const noteD = document.createElement("audio");
      noteD.src = "/assets/sounds/D.mp3";
      noteD.play();
    });

    const keyMi = document.getElementById("key-mi");
    keyMi.addEventListener("click", () => {
      const noteE = document.createElement("audio");
      noteE.src = "/assets/sounds/E.mp3";
      noteE.play();
    });

    const keyFa = document.getElementById("key-fa");
    keyFa.addEventListener("click", () => {
      const noteF = document.createElement("audio");
      noteF.src = "/assets/sounds/F.mp3";
      noteF.play();
    });

    const keySol = document.getElementById("key-sol");
    keySol.addEventListener("click", () => {
      const noteG = document.createElement("audio");
      noteG.src = "/assets/sounds/G.mp3";
      noteG.play();
    });

    const keyLa = document.getElementById("key-la");
    keyLa.addEventListener("click", () => {
      const noteA = document.createElement("audio");
      noteA.src = "/assets/sounds/A.mp3";
      noteA.play();
    });

    const keySi = document.getElementById("key-si");
    keySi.addEventListener("click", () => {
      const noteB = document.createElement("audio");
      noteB.src = "/assets/sounds/B.mp3";
      noteB.play();
    });

    const keyDoD = document.getElementById("key-do-d");
    keyDoD.addEventListener("click", () => {
      const noteDoD = document.createElement("audio");
      const uri = encodeURIComponent("/assets/sounds/C#.mp3");
      noteDoD.src = uri;
      noteDoD.play();
    });

    const keyReD = document.getElementById("key-re-d");
    keyReD.addEventListener("click", () => {
      const noteReD = document.createElement("audio");
      const uri = encodeURIComponent("/assets/sounds/D#.mp3");
      noteReD.src = uri;
      noteReD.play();
    });

    const keyFaD = document.getElementById("key-fa-d");
    keyFaD.addEventListener("click", () => {
      const noteFaD = document.createElement("audio");
      const uri = encodeURIComponent("/assets/sounds/F#.mp3");
      noteFaD.src = uri;
      noteFaD.play();
    });

    const keySolD = document.getElementById("key-sol-d");
    keySolD.addEventListener("click", () => {
      const noteSolD = document.createElement("audio");
      const uri = encodeURIComponent("/assets/sounds/G#.mp3");
      noteSolD.src = uri;
      noteSolD.play();
    });

    const keyLaD = document.getElementById("key-la-d");
    keyLaD.addEventListener("click", () => {
      const noteLaD = document.createElement("audio");
      const uri = encodeURIComponent("/assets/sounds/A#.mp3");
      noteLaD.src = uri;
      noteLaD.play();
    });
  },
};
</script>

<style lang="postcss" scoped>
.container-piano {
  background-color: #000000;
  border-radius: 10px;
  height: 276px;
  width: 531px;
  margin-top: 59px;
  display: flex;
  justify-content: space-between;
  padding: 10px;
  position: relative;
}
.key-white {
  background-color: #ffffff;
  width: 69px;
  cursor: pointer;
}
.key-white:nth-child(1) {
  border-radius: 5px 0px 0px 5px;
}
.key-white:nth-child(7) {
  border-radius: 0px 5px 5px 0px;
}
.key-white:active {
  background: #ffd12d;
}
.key-black {
  height: 184px;
  width: 30px;
  background-color: #000000;
  border-radius: 0px 0px 5px 5px;
  z-index: 1;
  position: absolute;
  cursor: pointer;
}
.key-black:active {
  background-color: #e6016f;
}
.key-black:nth-child(1) {
  left: 66px;
}
.key-black:nth-child(2) {
  left: 140px;
}
.key-black:nth-child(3) {
  left: 285px;
}
.key-black:nth-child(4) {
  left: 358px;
}
.key-black:nth-child(5) {
  left: 431px;
}

@media (max-width: 700px) {
  .container-piano {
    width: 368px;
  }
  .key-white {
    width: 47px;
  }
  .key-black {
    width: 20px;
  }
  .key-black:nth-child(1) {
    left: 49px;
  }
  .key-black:nth-child(2) {
    left: 98px;
  }
  .key-black:nth-child(3) {
    left: 198px;
  }
  .key-black:nth-child(4) {
    left: 248px;
  }
  .key-black:nth-child(5) {
    left: 298px;
  }
}

.container-note {
  display: flex;
  justify-content: space-around;
  width: 531px;
  margin-top: 48px;
  font-family: "PT Mono", monospace;
  color: rgba(255, 255, 255, 0.4);
}

@media (max-width: 700px) {
  .container-note {
    display: none;
  }
}
</style>