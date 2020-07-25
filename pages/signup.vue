<template>
    <div>
        <div class="panel border bg-white mx-auto mt-4 p-8">
            <div class="logo text-xl">
                <img class="mx-auto" src="/images/logo-xl.png" />
            </div>
            <div class="mt-2">
                <p class="text-center text-gray-500 font-semibold">Sign up to see photos and videos from your friends.</p>
                <button class="mt-4 rounded text-white w-full text-sm font-semibold py-1 blue-button">Log in with Facebook</button>
            </div>
            <hr class="mt-5" />
            <div class="mt-5">
                <input class="signup-input" type="text" placeholder="Mobile Number or Email">
                <input class="signup-input" type="text" placeholder="Full Name">
                <input class="signup-input" type="text" placeholder="Username">
                <input class="signup-input" type="text" placeholder="Password">
                <button class="mt-3 rounded text-white w-full text-sm font-semibold py-1 blue-button">Next</button>
            </div>
            <div class="text-center text-gray-500 text-xs mt-3">
                By signing up, you agree to our Terms . Learn how we collect, use and share your data in our Data Policy and how we use cookies and similar technology in our Cookies Policy .
            </div>
        </div>
        <div class="panel border bg-white mx-auto mt-2 p-8 text-sm text-center">
            Have an account? <span class="text-blue-500">Log in</span>
        </div>
    </div>
</template>

<script>
export default {
    layout: 'empty'
}
</script>

<style scoped>
.panel {
    max-width: 350px;
    width: 100%;
}

.logo > img {
    max-width: 150px;
    height: auto;
}

.blue-button {
    background: #0095f6;
}

.signup-input {
    @apply rounded;
    @apply border;
    @apply w-full;
    @apply p-2;
    @apply text-xs;
    background-color: #fafafa;
}

.signup-input:not(:first-of-type) {
    @apply mt-3;
}
</style>