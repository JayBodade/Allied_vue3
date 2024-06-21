<template>
    <tr>
        <td>
            <v-btn icon flat><v-icon color="red">mdi-close</v-icon></v-btn>
        </td>
        <td>
            <LookupComponent />
        </td>
        <td>
            <v-text-field density="compact" variant="underlined" flat></v-text-field>
        </td>
        <td>
            <v-text-field density="compact" variant="underlined" flat></v-text-field>
        </td>
        <td>Building</td>
        <td>
            <v-text-field density="compact" variant="underlined" flat></v-text-field>
        </td>
        <td>
            <v-text-field density="compact"  variant="underlined" flat></v-text-field>
        </td>
        <td>1.00</td>
        <td>
            <LookupComponent />
        </td>
        <td>
            <v-textarea density="compact" rows="1"></v-textarea>
        </td>
    </tr>
</template>
<script>
import LookupComponent from '../components/LookupComponent.vue';
export default {

    components: {
        LookupComponent
    }

}
</script>

<style></style>
