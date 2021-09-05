<template>
  <div>
     <!-- <div>
    <mainTable v-for="week in response">
      <row :meetings="week.dailyMeetings" />
    </mainTable>
  </div>



  //row
  
    <div v-for="meet on meetings">
      <span>{{ meet.name1 }} {{ meet.name2 }}</span>
    </div> -->
    






  </div>
</template>

<script>
import Vue from 'vue';
import axios from 'axios';
import VueAxios from 'vue-axios';

Vue.use(VueAxios, axios)

export default {
    name:"WeeksList",
    mounted(){
      Vue.axios.get('http://localhost:8080/api/getMeetings')  
      .then((resp)=>{
          console.warn(resp);
      }

      )
    }
}

</script>
