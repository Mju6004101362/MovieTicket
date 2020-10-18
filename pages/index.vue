<template>
  <div>
    <div class="searhBar">
      <input type="text" placeholder="ค้นหาภาพยนตร์" />
      <select id="" name="">
        <option value="">เลือกโรงภาพยนตร์</option>
        <option value="เซ็นทรัลเฟสติวัล เชียงใหม่">
          เซ็นทรัลเฟสติวัล เชียงใหม่
        </option>
        <option value="เซ็นทรัลแอร์พอร์ต เชียงใหม่">
          เซ็นทรัลแอร์พอร์ต เชียงใหม่
        </option>
      </select>
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.searhBar {
  height: 120px;
  display: grid;
  grid-template-columns: auto auto;
  grid-gap: 8px;
  justify-content: center;
  align-items: center;
  background-color: rgb(73, 73, 73);
}

.searhBar input,
.searhBar select {
  width: 200px;
  height: 40px;
  border-radius: 4px;
  border: none;
  padding: 0 12px;
}
.movieList {
  width: 1000px;
  margin: auto;
  padding: 32px 16px;
  background-color: rgb(73, 73, 73);
  border-radius: 4px;
}

.movieCard {
  width: 100%;
  height: 200px;
  border-radius: 4px;
  padding: 17px;
  display: grid;
  grid-template-columns: 10% auto auto;
  justify-content: flex-start;
}

.movieCard img {
  width: 109px;
  border-radius: 4px;
  object-fit: cover;
}

.movieCard .movieText {
  white-space: nowrap;
  width: 100%;
  overflow: hidden;
  text-overflow: ellipsis;
  text-align: center;
  color: #fff;
}

.movieCard button {
  width: 60px;
  border: none;
  border-radius: 4px;
  background-color: rgb(255, 238, 0);
  transition: 0.3s;
}

.movieCard h1,
.movieCard h3,
.movieCard p {
  color: #fff;
}

.movieCard button:hover {
  filter: brightness(0.8);
}
</style>
