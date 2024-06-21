<template>
    <div>
        <v-card style="min-height: 108px;">
            <v-card-text>
                <v-hover>
                    <template v-slot:default="{ isHovering, props }">
                        <div v-bind="props" style="height:83px;">
                            <v-combobox hide-details flat class="tagCombobox"
                                style="overflow-y: auto;height: 83px;width: 100% !important;" label="Combobox"
                                variant="solo" multiple
                                :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']">
                                <template v-slot:prepend-inner>
                                    <v-icon>mdi-tag</v-icon>
                                </template>
                                <template v-slot:append>
                                    <div v-if="edit" style="display: flex; width: 60px; justify-content: space-evenly; flex-direction: row;">
                                        <v-btn @click="edit = false" icon flat
                                            style="height: 25px; width: 25px; ">
                                            <v-icon style="font-size: 20px;" class="red--text">mdi-close</v-icon>
                                        </v-btn>
                                        <v-btn @click="edit = false" icon flat
                                            style="height: 25px; width: 25px;">
                                            <v-icon style="font-size: 20px;" class="blue--text">mdi-check</v-icon>
                                        </v-btn>
                                    </div>
                                    <v-btn v-else icon style="height: 25px; width: 25px;" flat>
                                        <v-icon v-show="isHovering" @click="edit = true" color="primary"
                                            style="font-size: 20px;">mdi-pencil</v-icon> 
                                    </v-btn>
                                </template>
                                <template v-slot:selection="{ item }">
                                    <v-chip color="blue" :input-value="selected" size="small">
                                        <v-icon size="small" left>mdi-label</v-icon>
                                        <span>{{ item.title }}</span>
                                        <v-icon v-if="edit" size="small">
                                            mdi-close
                                        </v-icon>
                                    </v-chip>
                                </template>

                            </v-combobox>
                        </div>

                    </template>
                </v-hover>
            </v-card-text>

        </v-card>
    </div>
</template>
<script>

export default {
    data() {
        return {
            edit: false,
        }
    }
}
</script>

<style>
.tagCombobox .v-text-field.v-text-field--solo .v-input__append-inner,
.v-text-field.v-text-field--solo .v-input__prepend-inner {
    align-self: start !important;
}

.tagCombobox {
    padding: 0px !important;
    margin: 0px !important;
}

.tagCombobox.v-text-field>.v-input__control>.v-input__slot:before,
.tagCombobox.v-text-field>.v-input__control>.v-input__slot:after {
    border: none !important;
}

.tagCombobox.v-select.v-select--chips.v-select--chips--small .v-select__selections {
    max-height: 76px;
    overflow-y: auto;
}

.v-color-picker__color {
    position: relative;
    height: 18px;
    max-height: 18px;
    width: 18px;
    margin: 2px 4px;
    border-radius: 30px;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    overflow: hidden;
    cursor: pointer;
}
</style>