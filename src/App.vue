<template>
  <div>
    <h1>Task 1</h1>
    <p v-for="user in users" :key="user.name">
      {{ user.name }} {{ user.surn }}
    </p>

    <h1>Task 2</h1>
    <ul>
      <li v-for="href in hrefs" :key="href.href">
        <a :href="href.href">{{ href.text }}</a>
      </li>
    </ul>

    <h1>Task 3</h1>
    <table>
      <tr v-for="product in products" :key="product.name">
        <td>{{ product.name }}</td>
        <td>{{ product.price }}</td>
        <td>{{ product.quantity }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [
        { name: 'name1', surn: 'surn1' },
        { name: 'name2', surn: 'surn2' },
        { name: 'name3', surn: 'surn3' }
      ],
      hrefs: [
        { href: '1.html', text: 'text1' },
        { href: '2.html', text: 'text2' },
        { href: '3.html', text: 'text3' }
      ],
      products: [
        { name: 'product1', price: 100, quantity: 5 },
        { name: 'product2', price: 200, quantity: 4 },
        { name: 'product3', price: 300, quantity: 3 }
      ]
    };
  }
};
</script>
