<template>
  <div class="lmarquee-example">
    <Lmarquee class="list">
      <marquee-item v-for="(item,i) in list" :key="i">{{item}}</marquee-item>
    </Lmarquee>
  </div>
</template>
<script type="text/ecmascript-6">
import Lmarquee from 'packages/lmarquee';
import marqueeItem from 'packages/marqueeItem';
export default {
  name: 'lmarquee-example',
  components: {
    Lmarquee,
    marqueeItem
  },
  data() {
    return {
      list: [
        'Javascript是世界上最好的语言1',
        'Javascript是世界上最好的语言2',
        'Javascript是世界上最好的语言3',
        'Javascript是世界上最好的语言4',
        'Javascript是世界上最好的语言5'
      ]
    };
  }
};
</script>
<style lang="less" scoped>
.lmarquee-example {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  .list {
    background-color: #cecece;
    color: #fff;
    li {
      width: 100%;
      height: 40px;
      line-height: 40px;
      text-align: center;
    }
  }
}
</style>
