<template>
  <div class="home">


      <!-- <FloorSB class="fbar"/> -->
       <div class="sb-container">
    <!-- <b-form-input v-model="text" placeholder="Input nama/nomer ruangan "></b-form-input> -->
        <b-form-input class="sbform" v-model="search" placeholder="Cari Ruangan "></b-form-input>
    <!-- <div class="mt-2">Value: {{ text }}</div> -->
  </div>

        <div v-for="item in filtered" :key="item.Id" class="card border-0 cardSpace" style="width: 18rem;">
        <router-link v-bind:to="'/mappage/'+item.Id" >
          <li class="list-group-item bg-light">Lantai {{item.Id}} </li>
          </router-link>
       </div>


   
         



        <!-- <div v-for="item in room" :key="item.Id" class="card border-0 cardSpace" style="width: 18rem;">
      
          <li class="list-group-item bg-light">Lantai {{item.id}} </li>
         
       </div> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import FloorList from '@/components/FloorList.vue'
// import FloorSB from '@/components/FloorSB.vue'
// import ruangan from  '@/assets/ruangan.json'
export default {
  name: 'ExploreView',
  components: {
    // FloorList,
    // FloorSB,
  },
  data() {
      return { 
        room : null,
        // Lantai: [{Id: "Lantai 1"},
        //         {Id:  "Lantai 2"},
        //         {Id:  "Lantai 3"},
        //         {Id:  "Lantai 4"},
        //         {Id:  "Lantai 5"},
        //         {Id:  "Lantai 6"},
        //         {Id:  "Lantai 7"},
        //         {Id:  "Basement"}],
         Lantai: [{Id: "1",
                  ruangan:["Lift", "Administrasi, "] },
                {Id:  "2",
                 ruangan:["Lift", "dosen","201"] },
                {Id:  "3",
                 ruangan:["Lift", "301"] },
                {Id:  "4",
                ruangan:["Lift", "401"]},
                {Id:  "5",
                ruangan:["Lift", "501"]},
                {Id:  "6",
                ruangan:["Lift", "601"]},
                {Id:  "7",
                ruangan:["Lift", "701"]},
                {Id:  "B1",
                ruangan:["satpam"]}],
        search:''
      }

    },
  methods: {
    say: function (msg) {
      return (msg)
    }
  },

    computed:{
     filtered:function(){
      //  return this.Lantai;
    return this.Lantai.filter((lantai)=>{
      // console.log(lantai.ruangan.length);
      // console.log(this.search)
      for(var i = 0; i < lantai.ruangan.length; i++)
{
        if(lantai.ruangan[i].indexOf(this.search) != -1)
        {
             console.log(lantai.ruangan[i])
            return(lantai.ruangan[i]);
             

        }
} 
      // return lantai.Id.match(this.search);
        // return lantai.ruangan.match(this.search); gabisa kalo object
    //        
    });
    }
   }
  // filtered:function(){
  //   return "aha"
  //   }
  //  }
}

</script>

<style scoped>


.cardSpace{
  /* width: 100%;*/
   background-color:#0E47A1 ;
}
.list-group-item{
  margin-bottom: 15px;
  height: 65px;
  border-radius: 10px;
  width: 98%;
  text-align: start;
  font-size: 32px;
  font-weight: bold;
 
}

.home{
  padding-top: 30px;
  display: flex;
  flex-direction: column;

  align-items: center;
}
.fbar{
  margin-bottom: 20px;
  min-width: 93%;
}
   .f-list{ 
/* display: flex;
  justify-content: center;
   flex-direction: row; */
    /* border: 5px solid red;  */
  min-width: 95%;
}


.sbform{
  border-radius: 30px;
}
</style>