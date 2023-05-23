<template>
	<div>
	  <div>{{ name }}</div>
	  <div>{{ surname }}</div>
	</div>
  </template>
  
  <script>
  export default {
	name: 'MyComponent',
	data() {
	  return {
		name: 'Nikita',
		surname: 'Kirkitskiy',
	  }
	},
  }
  </script>