<template>
    <div>
        <v-text-field v-model="date" density="compact"  variant="underlined" :label="label" @click="showDatePicker = true;"></v-text-field>
        <v-dialog v-model="showDatePicker" width="auto">
            <v-date-picker v-if="showDatePicker"  :modelValue="getDate" 
              @update:model-value="selectedDate" ></v-date-picker>
        </v-dialog>
    </div>
</template>
<script>

export default {
    props:['label'],
    data() {
        return {
            showDatePicker: false,
            date: null,
        }
    },
    methods: {
        selectedDate(val) {
            const dateObject = new Date(val);
            const day = dateObject.getDate();
            const month = dateObject.getMonth() + 1; // Months are zero-based in JavaScript
            const year = dateObject.getFullYear();

            this.date = `${day}/${month}/${year}`;
            this.showDatePicker = false;

        },


    },
    computed: {
        getDate() {
            let date;
            if (this.date) {
                const [day, month, year] = this.date.split('/').map(Number);
                date = new Date(year, month - 1, day);
            } else {
                date = new Date();
            }
            return [date];
        }


    },
}
</script>