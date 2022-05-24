<template>
  <div class="MapPage">
    <div>Id</div>
    <!-- <FloorSB class="fbar"/> -->
  <div class=upperBar>
      <h2>Lantai {{$route.params.Id}}</h2>
    <!-- <DropDRoomList/> -->
  </div>
      <!-- <FloorList class="f-list d-flex "/>  -->
    <div>
      <b-img src="../assets/lantai_7.png" fluid alt="Responsive image"></b-img>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

// import FloorList from '@/components/FloorList.vue'
// import FloorSB from '@/components/FloorSB.vue'
// import DropDRoomList from '@/components/DropDRoomList.vue'
export default {
  name: 'MapPage',
  components: {
 
    // FloorSB,
    // DropDRoomList,
  },
  data() {
      return { 
        id:this.$route.params.id,
        // Lantai: [{Id: "Lantai 1"},
        //         {Id:  "Lantai 2"},
        //         {Id:  "Lantai 3"},
        //         {Id:  "Lantai 4"},
        //         {Id:  "Lantai 5"},
        //         {Id:  "Lantai 6"},
        //         {Id:  "Lantai 7"},
        //         {Id:  "Basement"}],
        // search:''
      }

    },
  // created() {

  //   console.log(this.data);
    
  // },
  methods: {
    say: function (msg) {
      return (msg)
    }
  },
  // computed:{
    
  //    filtered:function(){
  //     //  return this.Lantai;
  //   return this.Lantai.filter((lantai)=>{
  //     console.log(lantai.Id);
  //     console.log(this.search)
  //     return lantai.Id.match(this.search);
  //   //        
  //   });
  //   }
  //  }
}
</script>

<style scoped>

.MapPage{
  padding-top: 30px;
  display: flex;
  flex-direction: column;
    gap: 15px;
  align-items: center;
}
.upperBar{
    display:flex;
    justify-content: space-between;

    /* border: 5px solid red; */
    color: white;
    width: 95%
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
</style>