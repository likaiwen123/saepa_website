<template lang="pug">
#contact
  .title 我们走过的道路
  .timeline
    timeline
  .title 我们的团队
  .structure
    .group
      .circle.
        项目中心
      .line |
      ul
        li 周末支教
        li 梦想课堂
        li 电脑传爱
        li 创新工作室
    .group
      .circle.
        对外交<br>流中心
      .line |
      ul
        li 设计工作室
        li 外宣部
    .group
      .circle.
        人力资<br>源中心
      .line |
      ul
        li 人力资源部
        li 撒爱工作室
</template>


<script>
import Timeline from '@/components/Timeline';
import pic1 from '@/images/1.jpg';
import pic2 from '@/images/2.jpg';

export default {
  name: 'mooc',
  components: {
    Timeline,
  },
  data() {
    return {
      time: {
        title: '我们走过的道路',
        src: pic1,
      },
      saepa11: {
        title: '我们的团队',
        src: pic2,
      },
    };
  },
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>

$size = 150px
#contact
  background url("../images/str.jpg") no-repeat center center
  background-attachment fixed
  -webkit-background-size cover
  -moz-background-size cover
  -o-background-size cover
  background-size cover

.timeline
  background white

.title
  mix-blend-mode screen
  font-size 50px
  font-weight bold
  background #30043f
  text-align center
  color whitesmoke
  padding 80px 60px
  text-shadow 1px 1px 1px #b838f9
.structure
  mix-blend-mode screen
  padding 50px 0
  background-color white
  display flex
  align-items flex-start
  justify-content space-around
  .group
    text-align center
    color #572c6c
    .line
      padding 20px 0
      color #572c6c
      font-weight bold
      font-size 25px
    .circle
      margin 0 auto
      background #572c6c
      height $size
      width $size
      font-size 30px
      display flex
      align-items center
      justify-content center
      border-radius 100%
      color white
    ul
      font-weight bold
      padding 0
      margin 0
      font-size 20px
      li
        padding 2px


@media only screen and (max-width 768px)
  #contact
    background-attachment scroll
  .title
    padding 60px
    font-size 35px
  .structure
    flex-direction column
    align-items center
    justify-content center
    .group
      padding 20px 0 50px 0
</style>
