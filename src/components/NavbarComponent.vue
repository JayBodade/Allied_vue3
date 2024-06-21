<template>
 <v-app-bar  app    class="allied-blue">
 
  <v-toolbar-title>
      <v-img class="shrink mt-1 " width="50"
        src="https://res.cloudinary.com/incquet-solution/image/upload/v1653605588/PROJECTS/ZOHO/CREATOR/Alliedsteel/logo.png"></v-img>
    </v-toolbar-title>
  
    <v-autocomplete
    class="mb-1  flex-grow-1 mr-4"
    width="40%"
    hide-no-data hide-details
  placeholder="Search by Potential Name"
  
  density="compact"
  bg-color="rgba(250,250,250,0.2)"
  flat
 
  :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
></v-autocomplete>

<v-tabs style="max-width: 650px;" v-model="activeTab">
      <v-tab href="#sales-kickoff">Overview</v-tab>
      <v-tab href="#acv">ACV</v-tab>
      <v-tab href="#amps">AMPS</v-tab>
      <v-tab href="#potentials">Global</v-tab>
      <v-tab href="#freight">Freight</v-tab>
      <v-tab href="#incident-log">Incident Log</v-tab>
    </v-tabs>
    <v-btn  icon :disabled="activeTab === 'amps'" >
      <v-icon>mdi-refresh</v-icon>
    </v-btn>
 </v-app-bar>

</template>
<script>
export default{
  data(){
    return{
      activeTab:null,
    }
  }
  
}
</script>

<style>
.allied-blue, .teal {
    background: #0076bf !important;
    color: white !important;
}

.nav-router-btn {
  text-decoration: none;

  padding: 0 16px;
  background-color: #272727;
  color: #ffffff !important;
  border-radius: 4px;
  height: 36px;
  min-width: 64px;
  display: inline-flex;
  align-items: center;
}
</style>