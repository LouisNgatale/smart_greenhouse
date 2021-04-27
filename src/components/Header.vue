<template>
  <div id="header">
        <div class="heading mx-4 pt-4">
            <div class="icon">
                  <img src="../assets/icons/cloud.svg" alt="">
            </div>
            <div class="status">
                <div class="date">{{ date }} </div>
                <div class="weather">Cloudy</div>
            </div>
        </div>
        <div class="container-fluid my-3">
            <div class="row px-2">
                <div class="col title">
                    <span>SMART GREENHOUSE DASHBOARD</span>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  computed: {
    date: function (){
       let today = new Date();
       let dd = String(today.getDate()).padStart(2, '0');
       let mm = String(today.getMonth());
       let day = today.getDay();

       let Months = [
         "January", "February", "March", "April", "May", "June",
         "July", "August", "September", "October", "November", "December"
       ];

       let Days = [
         "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"
       ]

       today = Months[mm] + " " + dd + ", " + Days[day];
       return today;
    }
  }
}
</script>

<style lang="scss">
.heading{
  display:flex;
  align-content: center;
  align-items: center;
  .icon{
    margin-right: 10px;
  }
  .weather{
    font-weight: bold;
  }
  
}
.title{
    font-weight: bold;
    font-size: 22px;
  }
</style>
