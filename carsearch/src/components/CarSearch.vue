<template lang="html">
  <div class="Root">
    <div id="wraper">
        <div class="but but1">
          <select class="js-example-basic-single" name="MAKE">
            <option value="AL">MAKE</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but2">
          <select class="js-example-basic-single" name="MODEL">
            <option value="AL">MODEL</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but3">
          <select class="js-example-basic-single" name="BODY_TYPE">
            <option value="AL">BODY TYPE</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but4">
          <select class="js-example-basic-single" name="PRICE">
            <option value="AL">PRICE</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but5">
          <select class="js-example-basic-single" name="YEAR">
            <option value="AL">YEAR</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but6">
          <select class="js-example-basic-single" name="LOCATION">
            <option value="AL">LOCATION</option>
            ...
            <option value="WY">Wyoming</option>
          </select>
        </div>
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
.but1 .select2-selection--single{
  border-top-right-radius: 0px !important;
  border-bottom-right-radius: 0px !important;
  border-top-left-radius: 5px !important;
  border-bottom-left-radius: 5px !important;
  border-color: rgb(221, 221, 221);
  border-right-width: 0px;
}
.but2 .select2-selection--single,.but3 .select2-selection--single,.but4 .select2-selection--single,
.but5 .select2-selection--single,.but6 .select2-selection--single{
  border-top-right-radius: 0px !important;
  border-bottom-right-radius: 0px !important;
  border-top-left-radius: 0px !important;
  border-bottom-left-radius: 0px !important;
  border-color: rgb(221, 221, 221);
  border-right-width: 0px;
}
.but .select2-container--default{
  width: 100%;
  height: 100%;
  margin-top: -2px;
  text-align: left;
}
.but .select2-selection--single{
  height: 100%;
  padding: 21px 10px;
}
.but .select2-selection__arrow{
  padding: 21px 10px;
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
