<template>
  <span className="user">
          <span className="name">{{ userData.name }}</span>
          <span className="handle">@{{ userData.handle }}</span>
        </span>
</template>

<script>

import { objectToString } from '@vue/shared';

export default {
 name: 'User',
  props: {
    userData: Object,
  },
}
</script>

<style>

</style>