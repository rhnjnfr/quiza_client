
import Signup from '~/components/signup.vue';

import LoginButton from '~/components/loginButton.vue';
<template>
    <div>
        <span class=" bg-teal-900 md:flex"><br class="md:flex"></span>
    </div>
    <header>
        <nav class="px-16 bg-white py-6 md:flex md:items-center drop-shadow-sm">
            <div class="flex justify-between items-center">
                <span class="text-black text-2xl cursor-pointer pr-10">
                    USER
                </span>
            </div>
            <div class="hidden lg:block lg:h-6 lg:w-px lg:bg-gray-900/10" aria-hidden="true" />
            <navigation />
            <div class="grid md:ml-auto gap-2 sm:grid-cols-1 md:grid-cols-2">
                <LoginButton/>
                <Signup />
            </div>
        </nav>
    </header>
    <main class=" py-2">
        <div class="mx-16 my-4">
            <slot />
        </div>
    </main>
</template>