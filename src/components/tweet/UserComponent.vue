<template>
  <img
    src="https://i.imgur.com/b-1EdHVV.jpg"
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
