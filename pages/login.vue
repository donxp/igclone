<template>
    <div>
        <div class="panel border bg-white mx-auto p-8">
            <div class="logo text-xl">
                <img class="mx-auto" src="/images/logo-xl.png" />
            </div>
            <div class="mt-5">
                <input class="signup-input" type="text" placeholder="Phone number, username or email">
                <input class="signup-input" type="text" placeholder="Password">
                <button class="mt-3 rounded text-white w-full text-sm font-semibold py-1 blue-button">Log In</button>
            </div>
            <hr class="mt-5" />
            <div class="mt-5 text-center text-sm text-blue-700 font-semibold">
                Log in with Facebook
            </div>
            <div class="mt-3 text-center text-xs">
                Forgot password?
            </div>
        </div>
        <div class="panel border bg-white mx-auto mt-2 p-8 text-sm text-center">
            Don't have an account? <span class="text-blue-500">Sign up</span>
        </div>
    </div>
</template>

<script>
export default {
    layout: 'empty'
}
</script>

<style scoped>
.panel:first-of-type {
    margin-top: 5rem;
}

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