<template>
  <div class="container-emoji">
    <img alt="GIF" id="imgGif">
  </div>
</template>

<script>
import { GiphyFetch } from "@giphy/js-fetch-api";
export default {
  GiphyFetch,
  mounted() {
    const emoji = async () => {
      const gf = new GiphyFetch("hoc7Xw81iwUP2iewXhekupQznVmYDlHK");
      const { data: gifs } = await gf.emoji({ sort: 'football', lang: 'fr', limit: 5 });
      console.log(gifs);
      console.log(gifs[0].embed_url)
      const gif = gifs[0].embed_url
      const image = document.getElementById('imgGif');
      image.setAttribute('src', gif);
    };
    emoji();
  },
};
</script>

<style lang="postcss" scoped>
.container-emoji {
  border: solid 1px blue;
  width: 200px;
  height: 200px;
  margin-top: 29px;
}
.container-emoji img {
  width: 100%;
  height: 100%;
}
</style>