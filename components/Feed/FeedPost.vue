<template>
    <div class="bg-white border flex flex-col">
        <div class="flex p-4 border-b items-center">
            <div>
                <img :src="'/images/' + post.profile_image" class="rounded-full w-8 h-8">
            </div>
            <div class="ml-4 flex justify-between flex-1 items-center">
                <div>
                    <span class="text-sm font-semibold">{{ post.name }}</span>
                </div>
                <div>
                    <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10.001 7.8C8.786 7.8 7.8 8.785 7.8 10s.986 2.2 2.201 2.2S12.2 11.215 12.2 10s-.984-2.2-2.199-2.2zm-7 0C1.786 7.8.8 8.785.8 10s.986 2.2 2.201 2.2S5.2 11.214 5.2 10s-.984-2.2-2.199-2.2zm14 0c-1.215 0-2.201.985-2.201 2.2s.986 2.2 2.201 2.2S19.2 11.215 19.2 10s-.984-2.2-2.199-2.2z"/></svg>
                </div>
            </div>
        </div>
        <div class="image-holder flex justify-center">
            <img class="w-full" :src="'/images/' + post.image">
        </div>
        <div style="padding: 10px 15px;">
            <div>
                <FeedPostButtons />
            </div>
            <div>
                likes
            </div>
        </div>
    </div>
</template>

<script>
import FeedPostButtons from './FeedPostButtons'

export default {
    components: { FeedPostButtons },
    props: ['post']
}
</script>

<style scoped>
.image-holder {
    max-height: 600px;
    max-width: 100%;
    margin-top: 1px;
}

.image-holder > img {
    width: auto;
    height: auto;
    max-width: 100%;
    max-height: 600px;
    object-fit: contain;
}
</style>