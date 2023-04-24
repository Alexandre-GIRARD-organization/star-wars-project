<script setup>
import FilmItem from "./components/FilmItem.vue";

const films = [
  {
    episode_id: 4,
    title: "A New Hope",
    director: "George Lucas",
    release_date: "1977-05-25",
  },
  {
    episode_id: 5,
    title: "The Empire Strikes Back",
    director: "Irvin Kershner",
    release_date: "1980-05-17",
  },
  {
    episode_id: 6,
    title: "Return of the Jedi",
    director: "Richard Marquand",
    release_date: "1983-05-25",
  },
  {
    episode_id: 1,
    title: "The Phantom Menace",
    director: "George Lucas",
    release_date: "1999-05-19",
  },
  {
    episode_id: 2,
    title: "Attack of the Clones",
    director: "George Lucas",
    release_date: "2002-05-16",
  },
  {
    episode_id: 3,
    title: "Revenge of the Sith",
    director: "George Lucas",
    release_date: "2005-05-19",
  },
];
</script>

<template>
  <main>
    <h1>Liste des films star wars:</h1>
    <ul id="liste_des_films_star_wars">
      <li
        v-for="film in films"
        :key="film.episode_id"
      >
        <FilmItem :film="film" />
      </li>
    </ul>
  </main>
</template>
