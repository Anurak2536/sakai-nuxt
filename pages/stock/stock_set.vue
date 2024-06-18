<template> 
    <h3>Bootstrap Table Example</h3>
    <table class="table">
      <thead>
        <tr>
          <th scope="col">ID</th>
          <th scope="col">Name</th>
          <th scope="col">Age</th>
          <th scope="col">City</th>
          <th scope="col">Active</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="person in persons" :key="person.id">
          <th scope="row">{{ person.id }}</th>
          <td>{{ person.name }}</td>
          <td>{{ person.age }}</td>
          <td>{{ person.city }}</td>
          <td>
            <button @click="cc1">1</button>
            <button @click="cc2">2</button>
          </td>
        </tr>
      </tbody>
    </table>  
</template>

<script> 
export default {
    name: 'stock_set',
    data() {
        return {
            nameNew: "เดอะบิว นิโมโร่", 
            persons: [
                { id: 1, name: 'John Doe', age: 30, city: 'New York' },
                { id: 2, name: 'Jane Smith', age: 25, city: 'Los Angeles' },
                { id: 3, name: 'Mike Johnson', age: 40, city: 'Chicago' }
            ]
        }
    },
    methods: {
        cc1(){
            alert('XXXXXXX1');
        },
        cc2(){
            alert('XXXXXXX2');
        }
    }
}
</script>

<style>

</style>