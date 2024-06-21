<template>
    <div class="mt-8">
        <h2 class="allied-blue-color-text">Building Codes & Loads</h2>
        <v-row class="deal-details-first-row mt-4">
            <v-col md="2" class="deal-details-first-col">
                <h4>Building Code</h4>
                <v-text-field variant="underlined" density="compact" hide-details>
                    <template v-slot:label>
                        Building Code <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-second-col">
                <h4>Ground Snow Load</h4>
                <v-text-field variant="underlined" density="compact" hide-details>
                    <template v-slot:label>
                        Roof Snow Load <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-third-col">
                <h4>Roof Snow Load</h4>
                <v-text-field variant="underlined" density="compact" hide-details>
                    <template v-slot:label>
                        Roof Snow Load <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-fourth-col">
                <h4>Roof Live Load</h4>
                <v-text-field variant="underlined" density="compact" hide-details>
                    <template v-slot:label>
                        Roof Live Load <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-fifth-col">
                <h4>Collateral Load</h4>
                <v-text-field density="compact" variant="underlined" hide-details>
                    <template v-slot:label>
                        Collateral Load <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-fifth-col">
                <h4>Dead Load</h4>
                <v-text-field density="compact" variant="underlined" hide-details label="Dead Load">

                </v-text-field>
            </v-col>
        </v-row>
        <v-row class="deal-details-first-row">
            <v-col md="2" class="deal-details-first-col">
                <h4>Wind Speed</h4>
                <v-text-field density="compact" variant="underlined" hide-details>
                    <template v-slot:label>
                        Wind Speed <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-second-col">
                <h4>Wind Exposure</h4>
                <v-text-field density="compact" variant="underlined" hide-details>
                    <template v-slot:label>
                        Wind Exposure<span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-third-col">
                <h4>Wind Enclosure</h4>
                <v-text-field density="compact" variant="underlined" hide-details>
                    <template v-slot:label>
                        Wind Enclosure <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-fourth-col">
                <h4>Seismic Parameters</h4>
                <v-text-field density="compact" variant="underlined" hide-details>
                    <template v-slot:label>
                        Seismic Design Category <span class="red--text">*</span>
                    </template>
                </v-text-field>
                <v-text-field density="compact" variant="underlined" label="Seismic Ss Parameter"
                    hide-details></v-text-field>
                <v-text-field density="compact" variant="underlined" label="Seismic S1 Parameter"
                    hide-details></v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-fifth-col">
                <h4>Seismic Site Class</h4>
                <v-text-field label="Soil Class"  density="compact" variant="underlined" hide-details>
                    <template v-slot:label>
                        Seismic Site Class <span class="red--text">*</span>
                    </template>
                </v-text-field>
            </v-col>
            <v-col md="2" class="deal-details-sixth-col">
                                <h4>Occupancy</h4>
                                <v-text-field   density="compact" variant="underlined"  hide-details>
                                    <template v-slot:label>
                                        Occupancy <span class="red--text">*</span>
                                    </template>
                                </v-text-field>
                            </v-col>

        </v-row>


    </div>
</template>
<script>
</script>