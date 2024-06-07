<script>
import Layout from '../Layout.vue'
import { Head } from '@inertiajs/vue3'

export default {
    props: {
        users: Object,
    }
}
</script>

<template>
    <Layout>
        <div class="flex flex-col gap-y-5">
            <div
                v-for="user in users" :key="`user-${user.id}`">
                <span>{{ user.name }}</span>
            </div>
        </div>
    </Layout>
</template>