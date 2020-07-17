<template>
    <div class="mt-6">
        <FeedPost v-for="(post, index) in feed" :key="index" :post="post" />
    </div>
</template>

<script>
import FeedPost from './FeedPost'

export default {
    components: { FeedPost },
    data() {
        return {
            feed: [
                {
                    name: 'profile101',
                    profile_image: 'profile-1.png',
                    image: 'post-1.png',
                    likes: 19,
                    description: 'Nature - cheaper than therapy.',
                    comments: [],
                    time_ago: '1 hour ago'
                },
                {
                    name: 'profile101',
                    profile_image: 'profile-1.png',
                    image: 'post-1.png',
                    likes: 19,
                    description: 'Nature - cheaper than therapy.',
                    comments: [],
                    time_ago: '1 hour ago'
                },
                {
                    name: 'profile101',
                    profile_image: 'profile-1.png',
                    image: 'post-1.png',
                    likes: 19,
                    description: 'Nature - cheaper than therapy.',
                    comments: [],
                    time_ago: '1 hour ago'
                }
            ]
        }
    }
}
</script>