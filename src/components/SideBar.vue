<template>
    <div>

         
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn v-bind="props"   position="fixed" icon  elevation="2" dark class="allied-blue" fab
                    style="bottom:640px;right: 15px;top: 70px" >
                    <v-icon>mdi-note-text</v-icon>
                </v-btn>
            </template>
            <span>Notes</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn v-bind="props"  position="fixed"   icon elevation="2" dark class="allied-blue" fab
                    style="bottom:570px; right: 15px;top:130px;">
                    <v-icon>mdi-calendar-check-outline</v-icon>
                </v-btn>
            </template>
            <span>Tasks</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn  v-bind="props"  position="fixed" icon  elevation="2" dark class="allied-blue" fab style="bottom:500px; right: 15px;top:190px;"
                   >
                    <v-icon>mdi-monitor</v-icon>
                </v-btn>
              
            </template>
            <span>Design Tracker</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template  v-slot:activator="{ props }">
                <v-btn v-bind="props"  position="fixed" icon elevation="2" dark class="allied-blue" fab
                    style="bottom:430px;right:15px;top:250px" target="_blank" >
                    <v-icon>mdi-alert-outline</v-icon>
                </v-btn>
            </template>
            <span>Add Incident</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template  v-slot:activator="{ props }">
                <v-btn v-bind="props" position="fixed" icon elevation="2" dark class="allied-blue" fab
                    style="bottom:360px;right:15px;top:310px">
                    <v-icon>mdi-google-drive</v-icon>
                </v-btn>
            </template>
            <span>Drive Link</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn v-bind="props" v-on="on"  position="fixed" icon  elevation="2" dark class="allied-blue" fab
                    style="bottom:290px;right:15px;top:370px" >
                    <v-icon>mdi-chart-timeline</v-icon>
                </v-btn>
            </template>
            <span>Timeline</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn v-bind="props" position="fixed" icon elevation="2" dark class="allied-blue" fab
                    style="bottom:220px;right:15px;top:430px;" 
                    target="_blank">
                    <v-icon>mdi-link</v-icon>
                </v-btn>
            </template>
            <span>Open Potential</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn v-bind="props"  position="fixed" icon elevation="2" dark class="allied-blue" fab
                    style="bottom:150px;right:15px;top:490px;" >
                    <v-icon>mdi-format-list-bulleted</v-icon>
                </v-btn>
            </template>
            <span>Building Highlights</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn  v-bind="props"   position="fixed" icon elevation="2" dark
                    class="allied-blue" fab style="bottom:80px;right:15px;top:550px;" >
                    <v-icon>mdi-currency-usd</v-icon>
                </v-btn>
                
            </template>
            <span>Running Cash Flow</span>
        </v-tooltip>
        <v-tooltip location="start">
            <template v-slot:activator="{ props }">
                <v-btn v-bind="props"  position="fixed" icon elevation="2" dark class="allied-blue" fab
                style="bottom:80px;right:15px;top:610px;"   >
                    <v-icon>mdi-calendar</v-icon>
                </v-btn>
            </template>
            <span>Project Schedule</span>
        </v-tooltip>
    </div>
 </template>

 <script>
 export default{

 }
</script>
