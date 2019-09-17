<template>
  <div>
    <label v-if="label">{{ label }}</label>
    <input :value="value" v-bind="$attrs" v-on="listeners" />
  </div>
</template>

<script type="text/javascript">
import { formFieldMixin } from '../mixins/formFieldMixin'
export default {
  mixins: [formFieldMixin]
}
</script>
