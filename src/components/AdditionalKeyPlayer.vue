<template>
    <div>
        <v-table>
            <thead>
                <tr>
                    <th>

                    </th>
                    <th class="text-left">
                        Name
                    </th>
                    <th class="text-left">
                        Relationship
                    </th>
                    <th>
                        Email
                    </th>
                    <th>
                        Phone
                    </th>
                    <th>
                        Company
                    </th>
                    <th>
                        Access Rights
                    </th>
                    <th>
                        Access Invite Status
                    </th>
                </tr>
            </thead>
            <tbody>
                <ContactItem v-for="item in desserts" :key="item.name" />
                <!-- <tr v-for="item in desserts" :key="item.name">
                    <td><v-btn flat icon> <v-icon color="red">mdi-close</v-icon></v-btn></td>
                    <td>{{ item.name }}</td>
                    <td>{{ item.calories }}</td>
                </tr> -->
            </tbody>
        </v-table>
    </div>
</template>
<script>
import ContactItem from '../components/ContactItem.vue';
export default {
    data() {
        return {
            desserts: [
                {
                    name: 'Frozen Yogurt',
                    calories: 159,
                },
                {
                    name: 'Ice cream sandwich',
                    calories: 237,
                },
                {
                    name: 'Eclair',
                    calories: 262,
                },
                {
                    name: 'Cupcake',
                    calories: 305,
                },
                {
                    name: 'Gingerbread',
                    calories: 356,
                },
                {
                    name: 'Jelly bean',
                    calories: 375,
                },
                {
                    name: 'Lollipop',
                    calories: 392,
                },
               
            ],
        }
    },
    components: {
        ContactItem
    }
}
</script>