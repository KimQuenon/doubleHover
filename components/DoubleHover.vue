<template>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 h-full">
        <div class="w-full h-full rounded-lg overflow-hidden relative p-2">
            <div class="bg-white rounded shadow backgroundScale h-full relative">
                <div class="rounded w-full h-full shadow-lg p-10 z-50 relative">
                    <div class="w-full h-full">
                        <h2 class="text-xl font-semibold mb-2">Card 1</h2>
                        <p class="text-gray-600">Tag 1</p>
                        <!-- <p class="text-gray-600">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero.</p> -->
                        <button class="bg-red-400 p-2 px-8 rounded-full text-white mt-4" type="button">See all</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.backgroundScale {
    position: relative;
}

.backgroundScale::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: url('/assets/images/qreative-agence-web-nivelles-hiwbi-2.webp');
    background-size: cover;
    transition: all 0.5s ease-in-out;
}

.backgroundScale:hover::before {
    transform: scale(0.8);
    height:70%;
}
</style>
