<template lang="html">
  <div class="Root">
    <div id="wraper">
         <div class="but but1">
          <select id="butt0" class="select2 mySelect0" name="MAKE">
            <option>MAKE</option>
            <option value="Toyota">Toyota</option>
            <option value="Nissan">Nissan</option>
            <option value="Mazda">Mazda</option>
            <option value="Honda">Honda</option>
            <option value="Ford">Subaru</option>
            <option value="Bmw">Bmw</option>
            <option value="Subaru">Subaru</option>
          </select>
        </div>
        <div class="but but2">
          <select id="butt1" class="select2 mySelect1" name="MODEL">
            <option value="MODEL">MODEL</option>
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but3">
          <select id="butt2" class="select2 mySelect2" name="BODY_TYPE">
            <option value="BODY TYPE">BODY TYPE</option>
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but4">
          <select id="butt3" class="select2 mySelect3" name="PRICE">
            <option value="PRICE">PRICE</option>
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but5">
          <select id="butt4" class="select2 mySelect4" name="YEAR">
            <option value="YEAR">YEAR</option>
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but6">
          <select id="butt5" class="select2 mySelect5" name="LOCATION">
            <option value="LOCATION">LOCATION</option>
            <option value="WY">Wyoming</option>
          </select>
        </div>
        <div class="but but7">
          <button type="button" class="searchButton" name="SEARCH">SEARCH</button>
        </div>
      </div>
      <div id="wraper2" v-show="moreFilters">
           <div class="but but1">
            <select id="butt6" class="select2 mySelect6" name="MAKE">
              <option>MAKE</option>
              <option value="Toyota">Toyota</option>
              <option value="Nissan">Nissan</option>
              <option value="Mazda">Mazda</option>
              <option value="Honda">Honda</option>
              <option value="Ford">Ford</option>
              <option value="Bmw">Bmw</option>
              <option value="Subaru">Subaru</option>
            </select>
          </div>
          <div class="but but2">
            <select id="butt7" class="select2 mySelect7" name="MODEL">
              <option value="MODEL">MODEL</option>
              <option value="WY">Wyoming</option>
            </select>
          </div>
          <div class="but but3">
            <select id="butt8" class="select2 mySelect8" name="BODY_TYPE">
              <option value="BODY TYPE">BODY TYPE</option>
              <option value="WY">Wyoming</option>
            </select>
          </div>
          <div class="but but4">
            <select id="butt9" class="select2 mySelect9" name="PRICE">
              <option value="PRICE">PRICE</option>
              <option value="WY">Wyoming</option>
            </select>
          </div>
          <div class="but but5">
            <select id="butt10" class="select2 mySelect10" name="YEAR">
              <option value="YEAR">YEAR</option>
              <option value="WY">Wyoming</option>
            </select>
          </div>
          <div class="but but6">
            <select id="butt11" class="select2 mySelect11" name="LOCATION">
              <option value="LOCATION">LOCATION</option>
              <option value="WY">Wyoming</option>
            </select>
          </div>
          <div class="but but7">
            <select id="butt12" class="select2 mySelect12" name="BODY_TYPE">
              <option value="BODY TYPE">BODY TYPE</option>
              <option value="WY">Wyoming</option>
            </select>
          </div>
        </div>
        <label @click='moreFilters = !moreFilters'>{{moreFiltersLabel()}}</label>
        <p>pusi ga strajo </p>
      </div>
</template>

<script>
export default {
  data: function(){
    return{
      moreFilters:false
    }
  },
  methods:{
    changeCss: function(){
      document.querySelector('.select2-search__field').style = 'border: 1px solid black;';
    },
    moreFiltersLabel: function(){
      if(this.moreFilters){
        return 'LESS FILTERS'
      }else{
        return 'MORE FILTERS'
      }
    }
  }
}
</script>
<style media="screen">
@font-face{
    font-family: "Gotham Pro";
    src: local("Gotham Pro Bold"), url("http://carvisor.co.nz/assets/fonts/GothaProBol.woff") format("woff");
    font-style: normal;
    font-weight: bold;
}
@font-face{
    font-family: "Gotham Pro Light";
    src: local("Gotham Pro Light"), url("http://carvisor.co.nz/assets/fonts/GothaProLig.woff") format("woff");
    font-style: normal;
}
.select2-results, .select2
{
  font-family: 'Gotham Pro Light', Arial, sans-serif;
}
.but select{
  height: 100%!important;
}
.but1 .select2-selection--single{
  border-top-right-radius: 0px ;
  border-bottom-right-radius: 0px ;
  border-top-left-radius: 5px ;
  border-bottom-left-radius: 5px ;
  border-color: rgb(221, 221, 221);
  border-right-width: 0px;
}
.but2 .select2-selection--single,.but3 .select2-selection--single,.but4 .select2-selection--single,
.but5 .select2-selection--single,.but6 .select2-selection--single{
  border-top-right-radius: 0px ;
  border-bottom-right-radius: 0px ;
  border-top-left-radius: 0px ;
  border-bottom-left-radius: 0px ;
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
  padding: 21px 0px 21px 10px;
}
.searchButton{
  width: 100%;
  height: 100%;
  color: white;
  background-color: rgb(243, 0, 95);
  border-top-right-radius: 5px ;
  border-bottom-right-radius: 5px ;
  border-top-left-radius: 0px ;
  border-bottom-left-radius: 0px ;
  border:0px solid white;
  padding-top: 2px;
}
.but7 .select2-selection--single{
  border-color: rgb(221, 221, 221);
  border-top-right-radius: 5px ;
  border-bottom-right-radius: 5px ;
  border-top-left-radius: 0px ;
  border-bottom-left-radius: 0px ;
}
@media only screen and (max-width: 1110px){
  .but1 .select2-selection--single{
    border-bottom: 0px solid white;
    border-bottom-left-radius: 0px;
  }
  .but5 .select2-selection--single{
    border-bottom-left-radius: 5px;
  }
  .but2 .select2-selection--single,.but3 .select2-selection--single{
    border-bottom: 0px solid white;
  }
  .but4 .select2-selection--single{
    border-right-width: 1px ;
    border-bottom-width: 0px;
    border-top-right-radius: 5px;
  }
  .searchButton{
    border-top-right-radius: 0px ;
  }
  .but7 .select2-selection--single{
    border-top-right-radius: 0px ;
  }
}
@media only screen and (max-width: 798px){
  .but1 .select2-selection--single{
    border-top-right-radius: 5px;
    border-right-width: 1px;
  }
  .but2 .select2-selection--single,.but3 .select2-selection--single,.but4 .select2-selection--single,
  .but5 .select2-selection--single,.but6 .select2-selection--single{
    border-top-right-radius: 0px ;
    border-bottom-right-radius: 0px ;
    border-top-left-radius: 0px ;
    border-bottom-left-radius: 0px ;
    border-color: rgb(221, 221, 221);
    border-right-width: 1px;
    border-bottom-width: 0px;
  }
  .searchButton{
    border-bottom-left-radius: 5px ;
  }
  .but7 .select2-selection--single{
    border-bottom-left-radius: 5px ;
  }
}
.select2-container--default .select2-results>.select2-results__options{
  max-height: 175px;
}
.select2-container--default .select2-selection--single .select2-selection__arrow b,
.pseudo-selection-arrow b
{
  display:none;
}
.select2-container--default .select2-results__option--highlighted[aria-selected] {
  background-color: #f0f2f5;
  border-bottom-color: #f0f2f5;
  color: #555;
}
.select2-results__options li {
  font-size: 13px;
  border-bottom: 1px solid #f0f2f5;
  padding-left: 15px;
  font-weight:400;
  color:rgb(85, 85, 85);
}
.select2-dropdown{
  border: 1px solid #ddd;
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
}
.select2.select2-container.select2-container--default.select2-container--below.select2-container--open.select2-container--focus{
  border-bottom: 1px solid #aaa !important;
}
.select2-selection__arrow i{
  vertical-align: text-bottom;
  margin-bottom:21px;
  -webkit-text-stroke: 1px white;
  color:#767676;
}
.select2.select2-container.select2-container--default:hover ,
.select2.select2-container.select2-container--default:hover .select2-selection__rendered,
.select2.select2-container.select2-container--default:hover i{
  color: #484848 !important;
}
.select2-selection__rendered{
  font-size: 14px;
  color:rgb(118, 118, 118)!important;
  font-weight: 600 !important;
  letter-spacing: 1px;
}
input::placeholder {
  font-size: 14px;
  color:rgb(118, 118, 118)!important;
  font-weight: 600 !important;
  letter-spacing: 1px;
  font-family: 'Gotham Pro Light', Arial, sans-serif;
}
.butt0.select2-dropdown.select2-dropdown--below,
.butt1.select2-dropdown.select2-dropdown--below,
.butt5.select2-dropdown.select2-dropdown--below{
  margin-top: -70px;
  background: transparent;
  border-top-left-radius: 5px;
}
.butt5 .select2-dropdown.select2-dropdown--below,
.butt1 .select2-dropdown.select2-dropdown--below{
  margin-top: -70px;
  background: transparent;
  border-top-left-radius: 0px;
}
.butt0 .select2-search.select2-search--dropdown,
.butt5 .select2-search.select2-search--dropdown,
.butt1 .select2-search.select2-search--dropdown{
  border: 0px solid transparent;
  border-top: 1px solid rgb(221, 221, 221);
  border-top-left-radius: 5px;
  height: 60px;
  padding-right: 25%;
  /* background-color: rgba(255, 255, 255,0.4); */
  background: transparent;
  border-bottom: 2px solid rgb(170, 170, 170);
}
.butt0 .select2-search__field,
.butt5 .select2-search__field,
.butt1 .select2-search__field{
  border: 0px solid transparent !important;
  height: 100%;
  width: 100%;
  /* background: transparent; */
  background-color: rgba(255, 255, 255,0.4);
  padding-left: 15px !important;
}
.butt0 .select2-results,
.butt5 .select2-results,
.butt1 .select2-results{
  margin-top: -1px;
  background: white;
}
</style>
<style lang="css" scoped>
:focus {
    outline:none;
}
.select2-container--default .select2-results__option--highlighted[aria-selected] {
  background-color: #f0f2f5;
  border-bottom-color: #f0f2f5;
  color: #555;
}
#wraper,#wraper2{
  display: grid;
  margin-top: 40px;
  grid-template-columns: repeat(55,1fr);
  grid-auto-rows: 70px;
  margin: 40px auto;
  width:90%;
  overflow-y: hidden;
  box-shadow:rgb(240, 240, 240) 0px 0px 13px 0px;
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
#wraper,#wraper2{
  width:780px;
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
#wraper,#wraper2{
  width:350px;
}
}
</style>
