<template>
    <div>
        <div class="text-sm font-semibold">
            {{ post.likes }} likes
        </div>
        <div>
            <div class="text-sm text-gray-500" v-if="post.comments.length > maxCommentSummary">
                View all {{ post.comments.length }} comments
            </div>
            <div class="text-sm" v-for="(comment, index) in commentSummary" :key="index">
                <span class="font-semibold">{{ comment.from }}</span> {{ comment.comment }}
            </div>
        </div>
        <div class="text-xxs uppercase font-semibold text-gray-500 mt-1">
            {{ post.time_ago }}
        </div>
    </div>
</template>

<script>
export default {
    props: ['post'],
    data() {
        return {
            maxCommentSummary: 3
        }
    },
    computed: {
        commentSummary() {
            const comments = []

            for(let i = 0; i < Math.min(this.post.comments.length, this.maxCommentSummary); i++) {
                comments.push(this.post.comments[i])
            }

            return comments
        }
    }
}
</script>