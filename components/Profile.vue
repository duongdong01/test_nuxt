<template>
  <div>
    <div class="flex justify-between h-[80px] border-y-[1px] items-center py-1">
      <h2 class="text-2xl font-bold">
        From Author's
      </h2>
      <div>
        <i class="fa-solid fa-arrow-left rounded-[50%] bg-[#f4f4f4] px-[18px] transition-all py-[16px] hover:bg-[#5138ee] hover:text-white" @click="arrowLeft()" /> <span>
          <i class="ml-2 fa-solid fa-arrow-right rounded-[50%] bg-[#f4f4f4] transition-all px-[18px] py-[16px] hover:bg-[#5138ee] hover:text-white" />
        </span>
      </div>
    </div>
    <a-carousel arrows>
      <div
        slot="prevArrow"
        class="custom-slick-arrow"
        style="left: 10px;zIndex: 1"
      >
        <a-icon type="left-circle" />
      </div>
      <div slot="nextArrow" class="custom-slick-arrow" style="right: 10px">
        <a-icon type="right-circle" />
      </div>
      <div><h3>1</h3></div>
      <div><h3>2</h3></div>
      <div><h3>3</h3></div>
      <div><h3>4</h3></div>
    </a-carousel>
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
/* For demo */
.ant-carousel >>> .slick-slide {
  text-align: center;
  height: 160px;
  line-height: 160px;
  background: #364d79;
  overflow: hidden;
}

.ant-carousel >>> .custom-slick-arrow {
  width: 25px;
  height: 25px;
  font-size: 25px;
  color: #fff;
  background-color: rgba(31, 45, 61, 0.11);
  opacity: 0.3;
}
.ant-carousel >>> .custom-slick-arrow:before {
  display: none;
}
.ant-carousel >>> .custom-slick-arrow:hover {
  opacity: 0.5;
}

.ant-carousel >>> .slick-slide h3 {
  color: #fff;
}
</style>
