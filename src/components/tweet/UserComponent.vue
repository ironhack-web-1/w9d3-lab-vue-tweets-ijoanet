<template>
  <span className="user">
    <span className="name">{{ name }}</span>
    <span className="handle">@{{ handle }}</span>
  </span>
</template>

<script>
export default {
  name: 'UserComponent',
  props: {
    name: {
      type: String,
      required: true,
    },
    handle: {
      type: String,
      required: true,
    },

  },
};
</script>
