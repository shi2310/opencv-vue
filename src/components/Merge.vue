<template>
  <div>
    <div class="pics">
      <div class="pic">
        <canvas ref="img1" />
        <p>
          <input
            type="file"
            @change="(e) => upload(e, 'img1')"
            accept="image/*"
          />
        </p>
      </div>
      <div class="pic">
        <canvas ref="canvas" class="img" />
      </div>
    </div>
    <p>
      <button @click="change">灰度图</button>
    </p>
  </div>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {};
  },
  precreate() {},
  created() {
    let info = this.$cv.getBuildInformation();
    console.log("main created", info, this.$cv);
  },
  methods: {
    upload(evt, refName) {
      let files = evt.target.files;
      if (!files.length) return;
      const canvas = this.$refs[refName];
      const ctx = canvas.getContext("2d");
      const imgurl = URL.createObjectURL(files[0]);
      const image = new Image();
      image.src = imgurl;
      image.onload = function(ev) {
        canvas.width = image.width;
        canvas.height = image.height;
        ctx.drawImage(image, 0, 0);
      };
    },
    change() {
      const img1 = this.$cv.imread(this.$refs.img1);
      let mat = new this.$cv.Mat();
      this.$cv.cvtColor(img1, mat, this.$cv.COLOR_RGBA2GRAY);
      this.$cv.imshow(this.$refs.canvas, mat);
      img1.delete();
      mat.delete();
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
.pics {
  display: flex;
  justify-content: space-between;

  .pic {
    width: calc(50% - 2px);
    border: 1px solid #dedede;
  }
}
</style>
