<script>
export default {
    props: {
        film: {
            type: Object,
            default: () => ({ 
            })
        }
    }
}
</script>

<template>
  <strong>{{ film.title }}</strong>, épisode {{ film.episode_id }}, <em>{{ film.release_date }}</em>, {{ film.director }}
</template>