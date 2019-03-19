<template>
  <div class="item">
    <div class="content">
      <div class="time-area">
        <div class="icon"></div>
        <div class="time">
          <span>{{time}}</span>
        </div>
      </div>
      <div class="note-area">
        <div class="note">
          <span>{{note}}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'list_item',
  props: ['time', 'note'],
  data () {
    return {
    }
  }
}
</script>

<style scoped>
  .item {
    height: 150rpx;
    width: 100%;
    margin-top: 5rpx;
    background-color: grey;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .content {
    height: 100%;
    width: 80%;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
</style>
