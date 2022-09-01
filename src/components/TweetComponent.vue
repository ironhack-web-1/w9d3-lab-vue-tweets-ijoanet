<template>
  <div className="tweet">
    <ProfileImage :image="user.image" />

    <div className="body">
      <div className="top">
        <User :name="user.name" :handle="user.handle" />
        <Timestamp :time="timestamp" />
      </div>

      <Message :message="message" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h" />
  </div>
</template>

<script>
import ProfileImage from './tweet/ProfileImageComponent.vue';
import User from './tweet/UserComponent.vue';
import Timestamp from './tweet/TimestampComponent.vue';
import Message from './tweet/MessageComponent.vue';
import Actions from './tweet/ActionsComponent.vue';

export default {
  name: 'TweetComponent',
  components: {
    ProfileImage,
    User,
    Timestamp,
    Message,
    Actions,
  },
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
