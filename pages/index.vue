<template>
  <div class="container-50 flex">
    <div class="feed mt-8">
      <UserStories />
      Feed
    </div>
    <div class="suggestions mt-8">
      <FeedSuggestions />
    </div>
  </div>
</template>

<script>
import UserStories from '../components/UserStories'
import FeedSuggestions from '../components/FeedSuggestions'

export default {
  components: { UserStories, FeedSuggestions }
}
</script>

<style scoped>
.feed {
  width: 66.6%;
}

.suggestions {
  width: 33.3%;
}
</style>
