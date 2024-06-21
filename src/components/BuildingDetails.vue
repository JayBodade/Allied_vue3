<template>
    <div class="mt-8">
        <h2 class="allied-blue-color-text">Building Details</h2>
        <v-row class="deal-details-first-row mt-4">
            <v-col md="4" class="deal-details-first-col">
                <h4>Dimensions</h4>
                <v-text-field density="compact" variant="underlined">
                    <template v-slot:label>
                        Width <span class="red--text">*</span>
                    </template>

                </v-text-field>
                <v-text-field density="compact" variant="underlined">
                    <template v-slot:label>
                        Length <span class="red--text">*</span>
                    </template>

                </v-text-field>
                <v-text-field density="compact" variant="underlined">
                    <template v-slot:label>
                        Height <span class="red--text">*</span>
                    </template>

                </v-text-field>
                <v-text-field density="compact" variant="underlined" label="Roof Pitch"></v-text-field>
                <v-select density="compact" variant="underlined" label="Pait System"
                    :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"></v-select>
            </v-col>
            <v-col md="4" class="deal-details-second-col">
                <h4>Roof Type</h4>
                <v-select density="compact" variant="underlined"
                    :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']">
                    <template v-slot:label>
                        Roof Type <span class="red--text">*</span>
                    </template>

                </v-select>
                <h4 class="mt-2">Roof Inso Type</h4>
                <v-text-field label="Roof Insulation" density="compact" variant="underlined"
                    hide-details></v-text-field>
            </v-col>
            <v-col md="4">

                <h4 class="mt-2">Wall Inso Type</h4>
                <v-text-field label="Wall Insulation" variant="underlined" density="compact"
                    hide-details></v-text-field>
            </v-col>
        </v-row>
        <v-row class="deal-details-first-row">
            <v-col md="4" class="deal-details-first-col">
                <h4>Framed Openings</h4>
             <v-text-field density="compact" variant="underlined" hide-details></v-text-field>
            </v-col>
            <v-col md="4" class="deal-details-second-col">
                <h4>Accessories</h4>
                <v-text-field density="compact" variant="underlined" hide-details></v-text-field>
            </v-col>
            <v-col md="4">
                                <h4>Doors Included</h4>
                                <v-text-field label="Walk Doors" density="compact" variant="underlined"   hide-details></v-text-field>
                                <!-- <v-text-field label="Roll Up Doors" v-model="deal.Roll_Up_Doors"
                                    hide-details></v-text-field> -->
                            </v-col>
        </v-row>

    </div>
</template>
<script>
export default {

}
</script>