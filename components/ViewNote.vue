<template>
  <div class="ViewNote">
    <small class="note">{{ note }}</small>
  </div>
</template>

<script type="ts">
import Vue from 'vue'

export default Vue.extend({
  Props: {
    note:{
      type: String,
      required: true
    }
  }
})
</script>
