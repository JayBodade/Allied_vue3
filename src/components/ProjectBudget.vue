<template>
    <div class="mt-8">
        <div style="display: flex;justify-content: space-between;">
            <h2 class="allied-blue-color-text">Project Budgets</h2>
            
        </div>
        <div>
                <v-table>
                    <thead>
                    <tr>
                        <th></th>
                        <th class="text-left">Material</th>
                        <th class="text-left">Estimated Weight</th>
                        <th class="text-left">Estimated Cost($)</th>
                        <th class="text-left">Product/Service Category</th>
                        <th class="text-left">Quantity</th>
                        <th class="text-left">Total($)</th>
                        <th class="text-left">Budget Cost/Lb($)</th>
                        <th class="text-left">Vendor</th>
                        <th class="text-left">Description</th>
                        <th class="text-left" >PO</th>
                    </tr>
                </thead>
                <tbody>
                   <SalesBudgetItem v-for="i in 5" :key="i" />
                </tbody>
                </v-table>
            </div>

    </div>

</template>

<script>
import SalesBudgetItem from '../components/SalesBudgetItem.vue';


    export default{
       components:{
        SalesBudgetItem
       }

    }
</script>