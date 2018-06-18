<template lang="pug">
  #app
    .header
      .navbar
        h1 HaveFun
        .searchbox
          i.fa.fa-search
          input(type="text" placeholder="Explore your own activities")
    .main
      .content
        .condition
          .condition-item.location
            h3  Location
            select#local(name="location")
              option(value="Taipei") 台北市
              option(value="Taipei") 台北市
              option(value="Taipei") 台北市
              option(value="Taipei") 台北市
              option(value="Taipei") 台北市
              option(value="Taipei") 台北市
              option(value="Taipei") 台北市
          .condition-item.date
            h3  Date
            .datebox
              label(for="") From
              input(type="date")
            br
            .datebox
              label(for="") To
              input(type="date")
          .condition-item.categories
            h3 Categories
            input(type="checkbox", name="a")
            |All
            br
            input(type="checkbox", name="a")
            |Entertainment
            br
            input(type="checkbox", name="a")
            |Food
            br
            input(type="checkbox", name="a")
            |Learning
            br
            input(type="checkbox", name="a")
            |Outdoors
        .show
          h1 Showing&nbsp
            span(style="color:#7828B4") 15
            | &nbspresults by ...
          .tagbox
            .tag
              span Koahsiung
              span.X X
          .show-item
            img(src="http://www.mottimes.com/image/report/8220120709165609.jpg", alt="")
            .show-content
              h2 Kogi Cosby sweater ethical.
              p Donec euismod scelerisque ligula. Maecenas eu varius risus, eu aliquet arcu. Curabitur fermentum suscipit est, tincidunt mattis lorem luctus id.
              span.host Ethan Foster
              span.tag Entertainment
              br
              span.loacl
                i.fas.fa-map-marker-alt
                |Kaohsiung City
              span.time
                i.far.fa-calendar-alt
                |2018/5/24 - 2018/5/31
          .show-item
            img(src="http://www.mottimes.com/image/report/8220120709165609.jpg", alt="")
            .show-content
              h2 Kogi Cosby sweater ethical.
              p Donec euismod scelerisque ligula. Maecenas eu varius risus, eu aliquet arcu. Curabitur fermentum suscipit est, tincidunt mattis lorem luctus id.
              span.host Ethan Foster
              span.tag Entertainment
              br
              span.loacl
                i.fas.fa-map-marker-alt
                |Kaohsiung City
              span.time
                i.far.fa-calendar-alt
                |2018/5/24 - 2018/5/31
          .show-item
            img(src="http://www.mottimes.com/image/report/8220120709165609.jpg", alt="")
            .show-content
              h2 Kogi Cosby sweater ethical.
              p Donec euismod scelerisque ligula. Maecenas eu varius risus, eu aliquet arcu. Curabitur fermentum suscipit est, tincidunt mattis lorem luctus id.
              span.host Ethan Foster
              span.tag Entertainment
              br
              span.loacl
                i.fas.fa-map-marker-alt
                |Kaohsiung City
              span.time
                i.far.fa-calendar-alt
                |2018/5/24 - 2018/5/31
          .page
            .page-item.pre
              i.fas.fa-angle-double-left
            .page-item.num 1
            .page-item.num 2
            .page-item.num 3
            .page-item.num 4
            .page-item.num 5
            .page-item.next
              i.fas.fa-angle-double-right

</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="sass">
  @import '/assets/helper/variables.sass'
  #app
    width: 100%
    height: 100%
    .header
      width: 100%
      height: 92px
      background-color: $color_purple
      display: flex
      justify-content: center
    .navbar
      display: flex
      max-width: 1200px
      width: 80%
      h1
        color: white
        margin-left: 78px
      .searchbox
        align-self: center
        border-bottom: 1px solid white
        padding-bottom: 5px
        margin-left: 149px
        width: 388px
        i
          font-size: 20px
          margin-right: 10px
          color: white
        input
          background-color: transparent
          border: none
          outline: none
          color: white
          width: 250px
          &::placeholder
            color: rgba(white,0.5)
    .main
      width: 100%
      display: flex
      justify-content: center
      .content
        max-width: 1200px
        width: 80%
        display: flex
        background-color: $color_l_grey
        .condition
          max-width: 300px
          .condition-item
            padding: 24px 40px
            padding-bottom: 24px
            border-bottom: 1px solid $color_t_grey
            background-color: $color_s_grey
            h3
              font-weight: bold
            &.location
              select
                width: 100%
            &.date
              .datebox
                display: flex
                justify-content: space-between
            &.categories
              border: none
              input
                margin-bottom: 10px
        .show
          margin-left: 42px
          display: flex
          flex-direction: column
          .tagbox
            margin-bottom: 24px
            .tag
              padding: 8px 16px
              display: inline-block
              border: 1px solid $color_light_purple
              color: $color_light_purple
              border-radius: 30px
              .X
                font-size: 5px
                margin-left: 10px
                cursor: pointer
          .show-item
            display: flex
            background-color: white
            margin-bottom: 24px
            img
              width: 220px
              height: 220px
            .show-content
              width: 560px
              padding: 24px 20px
              h2
                margin: 0
                color: $color_light_purple
              p
                line-height: 1.5
              .host
                font-weight: bold
                margin-right: 20px
              .tag
                display: inline-block
                margin-bottom: 14px
                padding: 3px 16px
                background-color: $color_t_grey
                color: white
                border-radius: 20px
                cursor: pointer
              .loacl
                margin-right: 20px
                color: $color_f_grey
                i
                  margin-right: 7px
                  color: black
              .time
                color: $color_f_grey
                i
                  margin-right: 7px
                  color: black
          .page
            display: flex
            justify-content: flex-end
            .page-item
              padding: 16px
              background-color: white
              color: $color_purple
              cursor: pointer
              &:hover
                background-color: $color_purple
                color: white
            .pre
              border-top-left-radius: 5px
              border-bottom-left-radius: 5px
            .next
              border-top-right-radius: 5px
              border-bottom-right-radius: 5px
            .num
              border-right: 1px solid $color_l_grey
              border-left: 1px solid $color_l_grey

</style>
