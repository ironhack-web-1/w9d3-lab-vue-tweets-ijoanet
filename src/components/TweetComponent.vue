<template>
  <div className="tweet">
    <img
      :src="user.image"
      className="profile"
      alt="profile"
    >

    <div className="body">
      <div className="top">
        <span className="user">
          <span className="name">{{ user.name }}</span>
          <span className="handle">@{{ user.handle }}</span>
        </span>

        <span className="timestamp">{{ timestamp }}</span>
      </div>

      <p className="message">
        {{ message }}
      </p>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment" />
        <i class="fas fa-retweet" />
        <i class="far fa-heart" />
        <i class="fas fa-share" />
      </div>
    </div>

    <i class="fas fa-ellipsis-h" />
  </div>
</template>

<script>
export default {
  props: {
    user: {
      type: Object,
      required: true,
    },
    timestamp: {
      type: String,
      default: 'Just now',
    },
    message: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
