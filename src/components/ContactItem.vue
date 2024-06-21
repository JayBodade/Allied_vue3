<template>
    <tr>
        <td>
            <v-btn icon flat>
                <v-icon color="red">mdi-close</v-icon>
            </v-btn>

        </td>
        <td>
            <ContactLookup/>
        </td>
        <td>
            <v-text-field density="compact" variant="underlined" value="designer"></v-text-field>
        </td>
        <td>
            <v-text-field density="compact" variant="underlined"  value="test@gmail.com"></v-text-field>
        </td>
        <td>
            <v-text-field density="compact" variant="underlined" value="1234567890"></v-text-field>
        </td>
        <td>
            <v-text-field density="compact" variant="underlined" value="test10"></v-text-field>
        </td>
        <td>
            <v-select density="compact" variant="underlined" :items="['View Only','Decision Maker']"></v-select>
        </td>
        <td>
            <v-btn color="blue" small variant="text" >ACCESS INVITE</v-btn>
        </td>
    </tr>
</template> 
<script>

import ContactLookup from '../components/ContactLookup.vue';
export default{
    data(){
        return{

        }
    },
    components:{
        ContactLookup
    }
}
</script>