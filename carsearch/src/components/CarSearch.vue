<template lang="html">
  <div class="Root">
    <div id="wraper">
        <div class="but but1">
          <select class="js-example-basic-single" style="height: 100%!important" name="MAKE">
            <option value="AL">Alabama</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but2">MODEL</div>
        <div class="but but3">BODY TYPE</div>
        <div class="but but4">PRICE</div>
        <div class="but but5">YEAR</div>
        <div class="but but6">LOCATION</div>
        <div class="but but7">SEARCH</div>
      </div>
  </div>
</template>

<script>
export default {
}
</script>
<style media="screen">
.but select{
  height: 100%!important;
}
</style>
<style lang="css" scoped>
#wraper{
  display: grid;
  margin-top: 40px;
  grid-template-columns: repeat(55,1fr);
  grid-auto-rows: 70px;
  margin: 40px auto;
  width:90%;
  border: 1px solid #777;
  border-radius: 5px;
  overflow-y: hidden;
}
.but{
  text-align: center;
  line-height: 70px;
  vertical-align: middle;
}
@media only screen and (min-width: 1110px){
.but1{
  grid-column: 1/8 ;
}
.but2{
  grid-column: 8/16 ;
}
.but3{
  grid-column: 16/24 ;
}
.but4{
  grid-column: 24/32 ;
}
.but5{
  grid-column: 32/40 ;
}
.but6{
  grid-column: 40/48 ;
}
.but7{
  grid-column: 48/56 ;
}
}
@media only screen and (max-width: 1110px){
.but1{
  grid-column: 1/14 ;
}
.but2{
  grid-column: 14/28 ;
}
.but3{
  grid-column: 28/42 ;
}
.but4{
  grid-column: 42/56 ;
}
.but5{
  grid-column: 1/21 ;
}
.but6{
  grid-column: 21/42 ;
}
.but7{
  grid-column: 42/56 ;
}
#wraper{
  width:790px;
}
}

@media only screen and (max-width: 798px){
.but1{
  grid-column: 1/56 ;
}
.but2{
  grid-column: 1/56 ;
}
.but3{
  grid-column: 1/56 ;
}
.but4{
  grid-column: 1/56 ;
}
.but5{
  grid-column: 1/56 ;
}
.but6{
  grid-column: 1/56 ;
}
.but7{
  grid-column: 1/56 ;
}
#wraper{
  width:350px;
}
}
</style>
