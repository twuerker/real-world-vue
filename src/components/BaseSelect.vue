<template>
  <div>
    <label v-if="label">{{ label }}</label>
    <select :value="value" v-bind="$attrs" v-on="listeners">
      <option v-for="option in options" :key="option">{{ option }}</option>
    </select>
  </div>
</template>

<script type="text/javascript">
import { formFieldMixin } from '../mixins/formFieldMixin'
export default {
  mixins: [formFieldMixin],
  props: {
    options: {
      type: Array,
      required: true
    }
  }
}
</script>
