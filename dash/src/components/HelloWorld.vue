<template>
  <div></div>
</template>

<script>
export default {

  data() { 
    return {
      orders:Object
    } 
  },
  mounted: function() {
    let api = 'https://api.konimbo.co.il/v1/items/?token=26699ce2c104def7accdca7f308036fa2e20bc8e2c01325ece975444ab139d7a&id=782612'
    this.axios.get(api).then((response) => {
      this.orders = response
      console.log(response.data)
    })
  },
  methods: {
    
  }
}
</script>