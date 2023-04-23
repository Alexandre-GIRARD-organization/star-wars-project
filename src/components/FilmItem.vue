<script>
export default {
    props: {
        film: Object
    }
}
</script>

<template>
    <strong>{{ film.title }}</strong>, épisode {{ film.episode_id }}, <em>{{ film.release_date }}</em>, {{ film.director }}
</template>