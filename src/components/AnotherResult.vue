<template>
    <div>
        <p>Counter is: {{ doubleCounter }}</p>
        <p>We clicked it: {{ stringCounter }}</p>
    </div>
</template>

<script>
import { mapGetters } from "vuex";

export default {
  computed: {
    ...mapGetters(["doubleCounter", "stringCounter"]),
    myField() {
      return 10;
    }
  }
};
</script>