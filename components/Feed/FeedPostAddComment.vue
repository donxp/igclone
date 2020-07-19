<template>
    <div class="border-t">
        <div class="flex p-4">
            <div class="w-11/12">
                <input class="text-sm" v-model="comment" type="text" placeholder="Add a comment...">
            </div>
            <div class="w-1/12">
                <div
                    class="text-sm text-center text-blue-200 font-semibold"
                    :class="{ 'text-blue-500': (comment.length > 0) }"
                >
                    Post
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            comment: ''
        }
    }
}
</script>