<template>
    <div>
        <div class="links text-xxs text-gray-500">
            <span>About</span>
            <span>API</span>
            <span>Jobs</span>
            <span>Help</span>
            <span>Privacy</span>
            <span>Terms</span>
            <span>Language</span>
        </div>
        <div class="mt-3 text-xxs text-gray-500">
            © 2020 IGCLONE
        </div>
    </div>
</template>

<style scoped>
.text-xxs {
    font-size: 0.7em;
}

.links > span:not(:first-of-type):before {
    content: '•';
    margin-right: 2px;
    font-size: 0.8em;
    text-align: center;
}
</style>