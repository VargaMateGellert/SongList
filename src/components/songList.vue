<template>
    <div>
        <table class="table">
            <thead>
                <tr>
                <td scope="col">Title</td>
                <td scope="col">Genre</td>
                <td scope="col">Year</td>
                <td scope="col">Time</td>
                </tr>
            </thead>
            <tbody>
                <tr v-for="song in props.songs">
                <td>{{ song.TITLE }}</td>
                <td>{{ song.GENRE }}</td>
                <td>{{ song.YEAR }}</td>
                <td>{{ song.TIME }}</td>
                </tr>

            </tbody>
        </table>
    </div>
</template>

<script setup>
const props = defineProps(['songs']);

</script>

<style scoped>

</style>