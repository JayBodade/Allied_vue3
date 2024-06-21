<template>
  <v-app >
    <NavbarComponent/>
    <v-main>
      <div style="width: 75%; margin: auto;">
        <v-container>
      <v-row dense>
       <v-col md="8">
        <BlueprintCard/>
       </v-col>
       <v-col md="4">
        <TagModule/>
       </v-col>
      </v-row>
      <DealDetails/>
      <StakeHolder/>
      <ProjectBudget/>
      <KeyPlayer/>
      <BuildingDetails/>
      <AdditionalNotes/>
      <BuildingCodesLoads/>
      <ScheduleComponent/>
      <SideBar/>
    </v-container>
   
    </div>
    
    </v-main>
    
  </v-app>
</template>

<script>

import ScheduleComponent from './components/ScheduleComponent.vue';
import AdditionalNotes from './components/AdditionalNotes.vue';
import KeyPlayer from './components/KeyPlayer.vue';
import ProjectBudget from './components/ProjectBudget.vue';
import NavbarComponent from './components/NavbarComponent.vue'
import BlueprintCard from './components/BlueprintCard.vue';
import TagModule from './components/TagModule.vue'
import DealDetails from './components/DealDetails.vue';
import StakeHolder from './components/StakeHolder.vue';
import BuildingDetails from './components/BuildingDetails.vue';
import BuildingCodesLoads from './components/BuildingCodesLoads.vue';
import SideBar from './components/SideBar.vue';
export default {
  name: 'App',

  components: {
    NavbarComponent,
    BlueprintCard,
    TagModule,DealDetails,StakeHolder,
    ProjectBudget,KeyPlayer,BuildingDetails,AdditionalNotes,
    BuildingCodesLoads,ScheduleComponent,SideBar
  },

  data: () => ({
    //
  }),
}
</script>

<style>
.allied-blue,
.teal {
  background: #0076bf !important;
}

.allied-blue--text {
  color: #0076bf !important;
}

.blue-bg {
  background-color: #3371b7 !important;
  color: #fff !important;
}

.lightBlue-bg {
  background-color: #deedf3;
}

.light2Blue-bg {
  background-color: #94b3de;
}

.orange-bg {
  background-color: #f5d5b8 !important;
}

.label-prepend .v-input__prepend-outer {
  width: 30%;
}

.red--text{
  color: red;
}
</style>
