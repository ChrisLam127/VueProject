<template>
  <div class="pagination">
    <button class="prev">Previous</button>
    <span class="middle">1</span>
    <span class="middle">...</span>
    <span class="middle">3</span>
    <span class="middle">4</span>
    <span class="middle active">5</span>
    <span class="middle">12</span>
    <span class="middle">13</span>
    <span class="middle">14</span>
    <span class="middle">15</span>
    <span class="middle">16</span>
    <span class="middle">...</span>
    <span class="middle">26</span>
    <button class="prev">Next</button>
  </div>
</template>

<script>
export default {
  name: "Pagination-Comp",
};
</script>

<style lang="scss" scoped>
@import "@/assets/_shared.scss";

.pagination {
  display: flex;
  justify-content: center;
  align-items: center;

  span {
    margin: 0 0.5rem;
    width: 30px;
    height: 30px;

    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    &:active {
      background: $blue;
    }
  }
  .prev {
    color: $blue;
    border: none;
  }
}
</style>
