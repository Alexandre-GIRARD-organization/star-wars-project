<script>
import formatDateMixin from './formatDateMixin';
export default {
    mixins: [formatDateMixin],
    props: {
        film: {
            type: Object,
            default: () => ({ 
            })
        }
    }
}
</script>

<!-- https://jerickson.net/how-to-format-dates-in-vue-3/ -->
<template>
  <strong>{{ film.title }}</strong>, épisode {{ film.episode_id }}, <em>{{ formatDate(film.release_date) }}</em>, {{ film.director }}
</template>