<script>
export default{
data(){
  return{
    arr: ['x', 'y', 'z'],
    arr1: [1, 2, 3],
  }
}
}
</script>

<template>
<div>{{ arr[0] }}</div>
<div>{{ arr[1] }}</div>
<div>{{ arr[2] }}</div>
<div>{{ arr1[0] + arr1[1] + arr1[2] }}</div>
</template>