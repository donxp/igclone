<template>
    <div class="p-4 flex flex-col">
        <div class="flex">
            <div>
                <img class="rounded-full w-16 h-16" src="/images/profile-0.png" />
            </div>
            <div class="flex flex-col justify-center ml-4">
                <span class="font-semibold text-sm">
                    username1
                </span>
                <span class="text-xs text-gray-500">
                    Don
                </span>
            </div>
        </div>
        <div class="mt-4">
            <div class="flex justify-between">
                <span class="text-gray-600 font-medium text-sm">Suggestions For You</span>
                <span class="text-xs font-semibold">See All</span>
            </div>
            <div v-for="(suggestion, index) in suggestions" :key="index" class="suggestion flex items-center">
                <img class="rounded-full w-8 h-8" :src="'/images/' + suggestion.image" />
                <div class="flex flex-col justify-start ml-2">
                    <span class="text-sm font-semibold">{{ suggestion.name }}</span>
                    <span class="text-xs text-gray-500">Followed by person1237 + 5 more</span>
                </div>
                <div class="flex justify-end flex-1">
                    <span class="text-xs text-blue-500 font-semibold">Follow</span>
                </div>
            </div>
        </div>
        <Footer class="mt-5" />
    </div>
</template>

<script>
import Footer from './Footer'

export default {
    components: { Footer },
    data() {
        return {
            suggestions: [
                {
                    name: 'janedoe137',
                    image: 'profile-5.png'
                },
                {
                    name: 'johndoe678',
                    image: 'profile-6.png'
                }
            ]
        }
    }
}
</script>

<style scoped>
.suggestion {
    margin-top: 12px;
}
</style>