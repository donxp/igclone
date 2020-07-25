<template>
    <div class="container-50 inbox border bg-white mt-4 rounded flex">
        <div class="message-list border-r">
            <div class="new-message border-b text-center font-semibold p-3">
                Direct
                <div class="new-message-button relative">
                    <svg class="w-6 h-6 absolute" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M18.174 1.826c-1.102-1.102-2.082-.777-2.082-.777L7.453 9.681 6 14l4.317-1.454 8.634-8.638s.324-.98-.777-2.082zm-7.569 9.779l-.471.47-1.473.5c-.104-.24-.234-.477-.498-.74-.264-.264-.5-.394-.74-.498l.5-1.473.471-.47s.776-.089 1.537.673c.762.761.674 1.538.674 1.538zM16 17H3V4h5l2-2H3c-1.1 0-2 .9-2 2v13c0 1.1.9 2 2 2h13c1.1 0 2-.9 2-2v-7l-2 2v5z"/></svg>
                </div>
            </div>
            <InboxMessageList :list="list" />
        </div>
        <div class="message">
            <InboxMessageWelcome />
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            list: [
                {
                    profile_image: 'profile-1.png',
                    username: 'janedoe137',
                    latest: 'Hello world',
                    ago: '2d'
                },
                {
                    profile_image: 'profile-2.png',
                    username: 'janedoe138',
                    latest: 'Hello world',
                    ago: '16w'
                }
            ]
        }
    }
}
</script>

<style scoped>
.inbox {
    min-height: 600px;
}

.message-list {
    width: 35%;
}

.message {
    width: 65%;
}

.new-message-button {
    left: 90%;
    bottom: 1.5rem;
}
</style>