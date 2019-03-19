<template>
  <div class="container">
    <div class="head">
      <div class="lhead">
        <div class="month" style="text-align:right;font-size:40px;">
          <span>{{day}}</span>
        </div>
      </div>
      <div class="rhead">
        <div class="month-en" style="text-align:left;font-size:20px;">
          <span>{{data}}</span>
          <br>
          <span>{{today}}</span>
        </div>
      </div>
    </div>
    <div class="body">
      <div class="data-scroll">
      </div>
      <item></item>
    </div>
  </div>
</template>

<script>
import item from '@/components/item.vue'

export default {
  data () {
    return {
      day: 19,
      data: '2019年3月',
      today: 'Wednesday'
    }
  },

  components: {
    item
  },

  methods: {
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .container {
    padding: 0rpx;
    margin: 0rpx;
    position:absolute;
    top: 0rpx;
    left: 0rpx;
    width:100%;
    height:100%;
    border:hidden;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }

  .head {
    height: 25%;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
  }

  .lhead{
    height: 100%;
    width: 30%;
    background-color: #FFEC8B;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
  }

  .rhead {
    height: 100%;
    width: 70%;
    background-color: #FFEC8B ;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
  }

  .month, .month-en {
    width: 90%;
    height: 40px;
    color: white;
  }

  .body {
    height: 75%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-content: center;
  }

  .data-scroll {
    height: 10%;
    width: 100%;
    background-color: dodgerblue;
  }
</style>
