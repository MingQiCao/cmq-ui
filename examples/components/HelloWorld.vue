<template>
  <div class="hello">
   <mq-btn :loading="loading" type="success" size="medium" @click="loadClick" >查询</mq-btn>
  </div>
</template>

<script>
export default {
  name: 'ButtonUse',
  data() {
    return {
      loading: false
    };
  },
  methods: {
    loadClick() {
        this.loading = true;
        setTimeout( () =>{
            this.loading = false;
        },2000)
    }
  }
}
</script>