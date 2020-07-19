<template>
    <div class="header">
        <div class="container-50">
            <div class="flex justify-between items-center">
                <div class="logo">
                    <img src="/images/logo.png">
                </div>
                <div class="search-bar">
                    <input type="text" placeholder="Search" class="border text-center rounded" />
                </div>
                <div class="header-controls flex">
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M18.672 11H17v6c0 .445-.194 1-1 1h-4v-6H8v6H4c-.806 0-1-.555-1-1v-6H1.328c-.598 0-.47-.324-.06-.748L9.292 2.22c.195-.202.451-.302.708-.312.257.01.513.109.708.312l8.023 8.031c.411.425.539.749-.059.749z"/></svg>
                    </div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M18.64 2.634C18.296 2.755 1.319 8.738.984 8.856c-.284.1-.347.345-.01.479.401.161 3.796 1.521 3.796 1.521l2.25.901s10.838-7.958 10.984-8.066c.148-.108.318.095.211.211-.107.117-7.871 8.513-7.871 8.513v.002l-.452.503.599.322s4.65 2.504 4.982 2.682c.291.156.668.027.752-.334.099-.426 2.845-12.261 2.906-12.525.079-.343-.148-.552-.491-.431zM7 17.162c0 .246.139.315.331.141.251-.229 2.85-2.561 2.85-2.561L7 13.098v4.064z"/></svg>
                    </div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M5.454 14.548s4.568-.627 6.518-2.576 2.576-6.518 2.576-6.518-4.569.627-6.518 2.576-2.576 6.518-2.576 6.518zm3.563-5.533c.818-.818 2.385-1.4 3.729-1.762-.361 1.342-.945 2.92-1.76 3.732-.543.545-1.426.545-1.969 0-.545-.543-.545-1.425 0-1.97zM10.001.4C4.698.4.4 4.698.4 10c0 5.303 4.298 9.601 9.601 9.601 5.301 0 9.6-4.298 9.6-9.601 0-5.302-4.299-9.6-9.6-9.6zM10 17.6c-4.197 0-7.6-3.402-7.6-7.6 0-4.197 3.402-7.6 7.6-7.6 4.197 0 7.601 3.402 7.601 7.6 0 4.197-3.404 7.6-7.601 7.6z"/></svg>
                    </div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17.19 4.156c-1.672-1.535-4.383-1.535-6.055 0L10 5.197 8.864 4.156c-1.672-1.535-4.382-1.535-6.054 0-1.881 1.726-1.881 4.519 0 6.245L10 17l7.19-6.599c1.88-1.726 1.88-4.52 0-6.245zm-1.066 5.219L10 15.09 3.875 9.375c-.617-.567-.856-1.307-.856-2.094s.138-1.433.756-1.999c.545-.501 1.278-.777 2.063-.777.784 0 1.517.476 2.062.978L10 7.308l2.099-1.826c.546-.502 1.278-.978 2.063-.978s1.518.276 2.063.777c.618.566.755 1.212.755 1.999s-.238 1.528-.856 2.095z"/></svg>
                    </div>
                    <div>
                        <img class="rounded-full border" src="/images/profile-0.png">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.header {
    @apply bg-white;
    @apply border-b;
}

.logo {
    padding: 12px 0;
}

.search-bar > input {
    background-color: #fafafa;
    font-size: 0.9em;
    padding: 2px 0;
}

.header-controls > div:not(:last-of-type) {
    margin-right: 20px;
}

.header-controls > div > svg {
    width: 28px;
    height: 28px;
    fill: currentColor;
}

.header-controls > div > img {
    width: 24px;
    height: 24px;
}
</style>