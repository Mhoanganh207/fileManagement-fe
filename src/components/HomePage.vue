<script setup>
import { useRouter } from 'vue-router';
import InputForm from './InputForm.vue';

const router = useRouter();

</script>

<template>

    <div class="w-screen h-screen flex p-48 items-center">
        <div class="w-1/2">
            <img width="600px" src="../assets/images/logo.png" alt="hero">

            <div class="p-14 pt-0 pr-0 font-bold text-slate-500 text-xl">Welcome to File Nest - Your Digital Organizer!
                Simplify your life with our intuitive file management
                solution. Effortlessly organize, access, and share your files from anywhere, anytime. Say goodbye to
                clutter and hello to efficiency with File Nest.</div>
        </div>

        <div class="flex w-1/2 flex-col space-y-5 items-center">
            <form class="flex w-[350px] flex-col space-y-5 items-center">
                <div class="w-full">
                    <p class="text-2xl float-start">Sign In</p>
                </div>
                <div>
                    <InputForm class="mt-1" Type="email" placeHolder="Email" />
                </div>
                <div>
                    <InputForm class="mt-1" Type="password" placeHolder="Password" />
                </div>

                <button class="bg-slate-600 text-white p-2 w-32 rounded-lg hover:bg-black duration-200">Log In</button>

                <div>
                    You don't have an account? <a @click="router.push('/signup')" class="text-slate-600 cursor-pointer">Sign Up</a>
                </div>

            </form>

        </div>
    </div>

</template>