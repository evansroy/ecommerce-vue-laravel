<script>
import GuestLayout from '../components/GuestLayout.vue'
export default {
    components: { GuestLayout },
    name: "ResetPassword"
}
</script>

<template>
    <div class="flex min-h-full flex-1 flex-col justify-center px-6 py-12 lg:px-8">

        <guest-layout title="Set New Password">
            <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">

                <form class="space-y-6" action="#" method="POST">

                    <div>
                        <div class="flex items-center justify-between">
                            <label for="new-password" class="block text-sm font-medium leading-6 text-gray-900">New
                                Password</label>

                        </div>
                        <div class="mt-2">
                            <input id="new-password" name="password" type="password" autocomplete="current-password"
                                required=""
                                class="block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                        </div>
                        <div class="flex items-center justify-between">
                            <label for="repeat-password" class="block text-sm font-medium leading-6 text-gray-900">Repeat
                                Password</label>

                        </div>
                        <div class="mt-2">
                            <input id="repeat-password" name="password" type="password" autocomplete="current-password"
                                required=""
                                class="block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                        </div>
                        <div class="text-sm">
                            <!-- <a href="#" class="font-semibold text-indigo-600 hover:text-indigo-500">Forgot password?</a> -->
                            <router-link to="/login" class="font-semibold text-indigo-600 hover:text-indigo-500">
                                Go back to LogIn?
                            </router-link>
                        </div>
                    </div>

                    <div>
                        <button type="submit"
                            class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Sign
                            in</button>
                    </div>
                </form>

            </div>
        </guest-layout>


    </div>
</template>


<style scoped></style>
