<template lang="pug">
.wrap
 .baApp_lay
  .baApp_head_org
   .baApp_head_mol
    .baApp_head_atm-logo
     h1
      | BE ArtisT.
     h2
      | 限界ドラムセッション
      br
      | 参加ページ

  .baApp_post_org
   .baApp_post_mol
    .baApp_post_atm-button
      router-link(to='/page2') Canvas

  .baApp_att_org
   .baApp_att_mol
    .baApp_att_atm
     p 下記操作説明をご確認ください↓

  .baApp_info_org
   .baApp_info_mol
    .baApp_info_atm-title 操作説明：
    .baApp_info_mol-list
     ol
      li Lorem ipsum dolor sit amet consectetur adipisicing.
      li Lorem ipsum dolor sit amet consectetur adipisicing.
      li Lorem ipsum dolor sit amet consectetur adipisicing.
      li Lorem ipsum dolor sit amet consectetur adipisicing.
      li Lorem ipsum dolor sit amet consectetur adipisicing.


</template>

<script>
export default {
}
</script>

<style lang="sass">
*
 margin: 0
 padding: 0

.wrap
  // background: #222
  background-image: url(https://picsum.photos/1600/1200/?image=158)
  background-size: cover
  width: 100%
  height: 100%
  .baApp
    &_lay
      padding: 20px
      // background-color: rgba(20,20,20,.7)
      background: linear-gradient(-45deg, rgba(29,93,35,.9), rgba(95,95,228,.8)),url(https://picsum.photos/1600/1200/?image=158) center center / cover no-repeat
      color: #f9f9f9
      max-width: 768px
      margin: auto
      height: 100vh
    &_head_org
      padding-top: 40px
    &_head_mol
    &_head_atm
      &-logo
        text-align: center
        h1
         font-size: 3em
         color: orange
        h2
         font-weight: 2em
         line-height: 1.7
    &_post
      &_org
        padding-top: 60px
      &_mol
        display: flex
        justify-content: center
      &_atm
        &-button
         padding: 0
         a
          color: #fff
          font-weight: 600
          text-decoration: none
          font-size: 2em
          background-color: darkorange
          border: 4px solid #fff
          border-radius: 15px
          padding: 20px 80px
          box-shadow: 0px 6px 0 #222
    &_att
      &_org
       margin-top: 45px
      &_mol
      &_atm
        text-align: center

    &_info
      &_org
       margin: 60px auto
       max-width: 96%
       // background-color: #666
      &_atm
        &-title
         font-size: 2em
         text-align: center
      &_mol-list
        display: flex
        justify-content: center
        ol
         padding-left: 2em
         margin-top: 10px
         li
          margin-bottom: 20px
          font-size: 1.2em
          line-height: 1.5

</style>
