<template>
    <div>
        <div v-for="(message, index) in list" :key="index" class="message">
            <div class="flex">
                <div>
                    <img :src="'/images/' + message.profile_image" class="rounded-full w-12 h-12">
                </div>
                <div class="ml-3 flex flex-col">
                    <span class="text-sm">{{ message.username }}</span>
                    <div class="flex">
                        <span class="text-sm text-gray-600 latest-message">{{ message.latest }}</span>
                        <span class="text-sm text-gray-600">{{ message.ago }}</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: ['list']
}
</script>
<style scoped>
.message {
    padding: 10px 16px;
}

.message:hover {
    @apply bg-gray-100;
}

.latest-message::after {
    content: '•';
    margin: 0 4px;
    font-size: 0.8em;
    text-align: center;
}
</style>