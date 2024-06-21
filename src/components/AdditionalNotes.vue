<template>

    <div class="mt-8">
        <h2 class="allied-blue-color-text">Additional Notes</h2>
        <div class="additional-notes">
            <div>
                <p>
                    <span style="font-weight: bold">Building Highlights</span>
                    (Project Notes)
                </p>
            </div>
            <div>
                <v-textarea variant="underlined" v-model="textArea" density="compact" auto-grow rows="2"
                    label="Building Highlights">
                </v-textarea>
            </div>
            <div style="padding: 15px 25px">
                <ul style="list-style-type: circle">
                    <li style="font-style: italic">
                        Note any pending items or notes from TSS here
                    </li>
                    <li style="font-style: italic">
                        Note what they want the building to look like
                    </li>
                    <li style="font-style: italic">
                        Any notes on the client themselves
                    </li>
                    <li style="font-style: italic">
                        Any future notes about the project
                    </li>
                    <li>
                        Other inclusions/design features the PM & TPM should know
                    </li>
                    <li>Any special considerations for loads</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            textArea: "kjsabsajkkheiuhnsajhksbcsnibcsnaubcnasiycvubsjvhycsakgjcfvsauhjcvasktscfvwcjsavhyahcsgvjyhcsavutjcvas ytfhvasucgsacvutacsfvygascghvcsatyfcsvagsacasuyyfvcsakafgcvsahgfcavcsakytfjcasajveykgawukjwnaiugkcbwjbvscgtfuascvvcsavgufkcsa",
        }
    }
}
</script>