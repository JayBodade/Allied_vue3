<template>
    <div class="mt-8">
        <h2 class="allied-blue-color-text">Stakeholder List</h2>
        <v-row class="deal-details-first-row mt-4">
            <v-col md="6" class="deal-details-first-col">
                <h4>Sales Person <span class="red--text">*</span></h4>
                <v-autocomplete density="compact" variant="underlined" :items="items" item-value="id" label="Potential Owner"
                    item-text="full_name"></v-autocomplete>
            </v-col>
            <v-col md="6">
                <v-select density="compact" variant="underlined" :items="items" label="PM Support"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="TPM Support"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="Drafting Resources"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="Checker"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="Logistics Coordinator"></v-select>
            </v-col>
        </v-row>
        <v-row class="deal-details-first-row ">
            <v-col md="6" class="deal-details-first-col">
                <h4>Project Team</h4>
                <v-autocomplete density="compact" variant="underlined" :items="items" item-value="id" item-text="full_name">
                    <template v-slot:label>
                        Estimator <span class="red--text">*</span>
                    </template>
                </v-autocomplete>
                <v-select density="compact" variant="underlined" :items="items" label="PM"> 
                    <v-select :items="items" label="PM"></v-select>
                    <v-select :items="items" label="TPM"></v-select>
                </v-select>
            </v-col>
            <v-col md="6">
                <h4>Project Team</h4>
                <v-select density="compact" variant="underlined" :items="items" label="Detailing Primary"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="Detailing Secondary"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="Stealing Engineer"></v-select>
                <v-select density="compact" variant="underlined" :items="items" label="Design Engineer"></v-select>
                
            </v-col>
        </v-row>
    </div>
</template>
<script>
export default {
    data() {
        return {
            items: ['india', 'china', 'russia', 'japan'],
        }
    }
}
</script>