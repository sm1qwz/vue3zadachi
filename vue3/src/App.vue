<script>
export default{
data(){
  return{
    hrefs: [
			{href: '1.html', text: 'text1'},
			{href: '2.html', text: 'text2'},
			{href: '3.html', text: 'text3'},
		],
    products: [
			{
				name: 'product1',
				price: 100,
				quantity: 5
			},
			{
				name: 'product2',
				price: 200,
				quantity: 4
			},
			{
				name: 'product3',
				price: 300,
				quantity: 3
			},
    ]
  }
},
methods: {
}
}
</script>

<template>
<ul>
    <li v-for="link in hrefs"><a href="{{ link.href }}">{{ link.text }}</a></li>
  </ul>
  <br>
  <br>
  <table>
    <tr v-for="col in products">
      <td>{{ col.name }}</td>
      <td>{{ col.price }}</td>
      <td>{{ col.quantity }}</td>
    </tr>
    </table>
</template>