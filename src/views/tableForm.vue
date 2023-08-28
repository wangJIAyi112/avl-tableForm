<template>
  <div class="hello">

    <avlForm :formConfig="formConfig"></avlForm>

    <avlTable :configData="item"></avlTable>
  </div>
</template>

<script>
import avlForm from '@/components/avl-form/avl-form'

import avlTable from '@/components/avl-table/avl-table'



export default {
  name: 'HelloWorld',
  components: {
    avlForm,
    avlTable

  },
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      formConfig: [{ id: 1,propName: 'contract',type: 'avl-input',size: 'small' ,defaultValue: '',placeholder: '',}]
    }
  }
}
</script>

<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
