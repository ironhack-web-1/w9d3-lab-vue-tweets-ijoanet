<template>
  <img
    :src="image"
    className="profile"
    alt="profile"
  >
</template>

<script>
export default {
  name: 'ProfileImageComponent',
  props: {
    image: {
      type: String,
      required: true,
    },
  },
};
</script>
