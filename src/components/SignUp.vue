<script setup>
import InputForm from './InputForm.vue';

</script>

<template>

<section class="bg-gray-50  font-bold">
        <div class="flex flex-col items-center justify-center px-6 py-8 mx-auto md:h-screen lg:py-0">
            <a href="#" class="flex items-center mb-6 text-2xl font-semibold text-gray-900 dark:text-white">
                <img class="w-96" src="../assets/images/logo.png" alt="logo">
            </a>
            <div
                class="w-full bg-white rounded-lg shadow dark:border md:mt-0 sm:max-w-md xl:p-0  dark:border-gray-700">
                <div class="p-6 space-y-4 md:space-y-5 sm:p-8">
                    <h1 class="text-xl font-bold leading-tight tracking-tight text-gray-900 md:text-2xl ">
                        Create account
                    </h1>
                    <form class="space-y-3 md:space-y-6" action="#">
                        <div class="flex space-x-2">
                            <InputForm class="w-full" Type="text" placeHolder="Name" />
                        </div>
                        <div>
                            <InputForm class="w-full" Type="email" placeHolder="Email" />
                        </div>
                        <div>
                            <InputForm class="w-full" Type="password" placeHolder="Password" />
                        </div>
                        
                        <div class="flex items-start">
                            <div class="flex items-center h-5">
                                <input id="terms" aria-describedby="terms" type="checkbox"
                                    class="w-4 h-4 border border-gray-300 rounded bg-gray-50 focus:ring-3 focus:ring-pink-300 text-pink-300"
                                    required>
                            </div>
                            <div class="ml-3 text-sm">
                                <label for="terms" class=" text-gray-500 dark:text-gray-300">I accept the <a
                                        class="text-primary-600 hover:underline dark:text-primary-500" href="#">Terms and
                                        Conditions</a></label>
                            </div>
                        </div>
                        <button @click.prevent="signUp" type="submit"
                            class="w-full text-white bg-slate-400 font-bold hover:bg-primary-700 focus:ring-4 focus:outline-none focus:ring-slate-300 rounded-lg text-md px-5 py-2.5 text-center">Create
                            an account</button>

                    </form>
                </div>
            </div>
        </div>
    </section>

</template>