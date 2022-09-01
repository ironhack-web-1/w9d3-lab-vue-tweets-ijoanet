<template>
  <span className="timestamp">{{ time }}</span>
</template>

<script>
export default {
  name: 'TimestampComponent',
  props: {
    time: {
      type: String,
      required: true,
    },

  },
};
</script>
