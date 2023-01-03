<script setup>

import { ref } from 'vue';

import User from './User.vue';
import Message from './Message.vue';
import Timestamp from './Timestamp.vue';
import ProfileImage from './ProfileImage.vue';
import Actions from './Actions.vue';

const props = defineProps(["tweet"])

</script>
<template>
<div className="tweet">
  <ProfileImage :image="tweet.user.image" />
  

    <div className="body">
      <div className="top">
        <span className="user">
        <User :name="tweet.user.name" :handle="tweet.user.handle"/>
        </span>

        <Timestamp :timestamp="tweet.timestamp" />
      </div>

      <Message :message="tweet.message" />

     <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
