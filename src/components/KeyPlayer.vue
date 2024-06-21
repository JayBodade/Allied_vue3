<template>
    <div class="mt-8">
        <div style="display: flex;justify-content: space-between;">
            <h2 class="allied-blue-color-text">Key Players</h2>
            <v-btn color="primary"> Update
                Access Endorsements </v-btn>
        </div>
        <AdditionalKeyPlayer/>

    </div>
</template>
<script>
import AdditionalKeyPlayer from '../components/AdditionalKeyPlayer.vue';
export default{
    components:{
        AdditionalKeyPlayer
    }
}
</script>