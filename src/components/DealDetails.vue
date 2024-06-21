<template>
    <div class="mt-4">
        <h2 class="allied-blue-color-text">Project Information</h2>
        <v-row class="deal-details-first-row mt-4">
            <v-col md="4" class="deal-details-first-col">
                <h4>Project Name <span style="color: red;">*</span></h4>
                <v-text-field density="compact" variant="underlined" hide-details required value="402423 : ACV Test" ></v-text-field>
            </v-col>
            <v-col md="4" class="deal-details-second-col">
                <h4>Account Name <span style="color: red;">*</span></h4>
                <LookupComponent class="mt-2" Entity="Accounts" itemText="Account_Name" required itemValue="id"
                    itemKey="Account_Name" />
            </v-col>
            <v-col md="4">
                <h4>Allied Job No.</h4>
                <v-text-field  density="compact" variant="underlined" value="30" hide-details></v-text-field>
            </v-col>
            
        </v-row>
        <v-row class="deal-details-first-row">
                <v-col md="4" class="deal-details-first-col">
                    <h4>Project Shipping Address</h4>
                    <v-tabs v-model="tab" hide-slider :show-arrows="false">
                        <v-tab href="#building">Building</v-tab>
                        <v-tab href="#shipping">Shipping</v-tab>
                        <v-tab href="#billing">Billing</v-tab>
                    </v-tabs>

                    <v-tabs-window v-model="tab">
                        <v-tabs-window-item value="building">
                            <v-text-field density="compact" variant="underlined" required hide-details>
                                <template v-slot:label>
                                    Building Address <span class="red--text">*</span>
                                </template>
                            </v-text-field>
                            <v-text-field density="compact"  variant="underlined" required hide-details>
                                <template v-slot:label>
                                    Building City <span class="red--text">*</span>
                                </template>
                            </v-text-field>
                            <v-text-field density="compact" variant="underlined" required hide-details>
                                <template v-slot:label>
                                    Building State <span class="red--text">*</span>
                                </template>
                            </v-text-field>
                            <v-text-field density="compact" variant="underlined" required hide-details>
                                <template v-slot:label>
                                    Building Zip Code <span class="red--text">*</span>
                                </template>
                            </v-text-field>
                            <v-text-field density="compact" variant="underlined" required hide-details>
                                <template v-slot:label>
                                    Building Country <span class="red--text">*</span>
                                </template>
                            </v-text-field>
                        </v-tabs-window-item>

                        <v-tabs-window-item value="shipping">
                            <v-text-field density="compact" variant="underlined" label="Shipping Address" required hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="Shipping City" required hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="Shipping State" required hide-details></v-text-field>
                            <v-text-field  density="compact" variant="underlined" label="Shipping Zip Code" required hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="Shipping Country" required hide-details></v-text-field>
                        </v-tabs-window-item>

                        <v-tabs-window-item value="billing">
                            <v-text-field  density="compact" variant="underlined" label="Billing Street" hide-details></v-text-field>
                            <v-text-field  density="compact" variant="underlined" label="Billing City" hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="Billing Zip Code" hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="County" hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="Billing State" hide-details></v-text-field>
                            <v-text-field density="compact" variant="underlined" label="Billing Country" hide-details></v-text-field>
                        </v-tabs-window-item>
                    </v-tabs-window>

                    <v-checkbox label="Project Address different from Shipping Address" hide-details></v-checkbox>
                    <v-checkbox label="Project Address different from Billing Address"></v-checkbox>
                </v-col>
                <v-col md="4" class="deal-details-second-col">
                    <h4>Desired Delivery Date</h4>
                    <CustomInput label="Delivery Deadline" />
                    <CustomInput label="Desired Approval Drawing Date" />
                    <CustomInput label="Column Placement Plans" />
                    <h4 class="mt-2">Payment Terms</h4>
                    <v-select density="compact" class="custom-select" variant="underlined" :items="items" item-value="display_value" item-text="display_value"
                        hide-details>
                        <template v-slot:label>
                            Payment Terms <span class="red--text">*</span>
                        </template>
                    </v-select>
                    <v-text-field density="compact" variant="underlined" label="Special Payment Terms" hide-details>
                        <template v-slot:label>
                            Special Payment Terms
                        </template>
                    </v-text-field>
                    <v-select density="compact" :items="items" variant="underlined" item-value="display_value" item-text="display_value" required hide-details>
                        <template v-slot:label>
                            Special Contract/Terms<span class="red--text">*</span>
                        </template>
                    </v-select>
                    <v-select density="compact" label="Bond/Lien" variant="underlined" :items="items" required item-text="display_value" hide-details>
                        <template v-slot:label>
                            Bond/Lien<span class="red--text">*</span>
                        </template>
                    </v-select>
                    <v-select density="compact" label="Credit Insurance" variant="underlined" :items="items" item-value="display_value"
                        item-text="display_value" required hide-details>
                        <template v-slot:label>
                            Credit Insurance<span class="red--text">*</span>
                        </template>
                    </v-select>
                    <v-select  density="compact" label="Tax Exempt" variant="underlined" :items="items" item-value="display_value" item-text="display_value"
                        hide-details>
                        <template v-slot:label>
                            Tax Exempt
                        </template>
                    </v-select>
                </v-col>
                <v-col md="4">
                    <h4>Project Details</h4>
                    <v-text-field density="compact" variant="underlined" label="Cost" type="number" prepend-icon="mdi-currency-usd" hide-details>
                        <template v-slot:label>
                            Total Budget Cost
                        </template>
                    </v-text-field>
                    <v-select density="compact" label="Complexity"  variant="underlined" :items="items" item-value="display_value" item-text="display_value"
                        required hide-details>
                        <template v-slot:label>
                            Complexity<span class="red--text">*</span>
                        </template>
                    </v-select>
                    <v-select density="compact" label="Industry" variant="underlined" :items="items" item-value="display_value" item-text="display_value"
                        hide-details>
                        <template v-slot:label>
                            Industry<span class="red--text">*</span>
                        </template>
                    </v-select>
                    <v-select density="compact" label="Software" variant="underlined" :items="items" item-value="display_value" item-text="display_value"
                        hide-details></v-select>
                    <v-text-field  density="compact" label="MBS Quote" variant="underlined" hide-details></v-text-field>
                    <v-textarea density="compact" variant="underlined" label="Building Use" rows="2" required 
                        hide-details>
                        <template v-slot:label>
                            Building Use<span class="red--text">*</span>
                        </template>
                    </v-textarea>
                </v-col>

            </v-row>
    </div>
</template>

<script>
import LookupComponent from '../components/LookupComponent.vue';
import CustomInput from "../components/CustomInput.vue";
export default {
    data() {
        return {
            tab: 'building',
            items: ['india', 'usa', 'russia', 'china', 'japan'],
        }

    },
    components: {
        LookupComponent, CustomInput
    }
}

</script>

<style>
.allied-blue-color-text {
    color: #0076bf;
}

.deal-details-first-row {
    border: 1px solid black;
}

.deal-details-second-row {
    margin: 0px !important;
}

.deal-details-second-row,
.deal-details-third-row {
    border: 1px solid black;
    border-top: 0;
}

.deal-details-first-col,
.deal-details-second-col,
.deal-details-third-col,
.deal-details-fourth-col,
.deal-details-fifth-col {
    border-right: 1px solid black;
}

.additional-notes {
    border: 1px solid black;
    padding: 10px;
}

.additional-notes,
.deal-details-first-row,
.deal-details-second-row,
.deal-details-third-row {
    background: #fff;
}

.drive {
    padding: 8px;
}

.drive iframe {
    border: 1px solid #ddd;
    border-radius: 3px;
}

.v-input .v-label {
    height: 35px !important;
}



.v-input__control {
    min-height: 10px !important;
}
</style>
