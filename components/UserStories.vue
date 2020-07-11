<template>
    <div class="border bg-white rounded-sm">
        <div class="flex p-5">
            <div v-for="(story, index) in stories" :key="index" class="story flex justify-center flex-col">
                <img
                    :src="'/images/' + story.image"
                    class="rounded-full w-16 h-16 gradient-border" />
                <span class="text-center text-xs">{{ story.name }}</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            stories: [
                {
                    name: 'user1',
                    image: 'profile-1.png'
                },
                {
                    name: 'user2',
                    image: 'profile-2.png'
                }
                ,
                {
                    name: 'user3',
                    image: 'profile-3.png'
                }
                ,
                {
                    name: 'user4',
                    image: 'profile-4.png'
                }
            ]
        }
    }
}
</script>

<style scoped>
.story:not(:first-of-type) {
    margin-left: 16px;
}

.gradient-border {
    border: double 3px transparent;
    background-image: linear-gradient(white, white), radial-gradient(circle at top right, #c21b80,#fa9f4d);
    background-origin: border-box;
    background-clip: content-box, border-box;
}
</style>