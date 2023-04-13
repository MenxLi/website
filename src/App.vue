<script setup>
import ShortBio from './components/ShortBio.vue'
import Publications from './components/Publications.vue'
import MoreSites from './components/MoreSites.vue'
</script>

<template>
  <ShortBio></ShortBio>
  <Publications></Publications>
  <MoreSites></MoreSites>
</template>

<style>
h3.subtitle{
    font-family: Inter, system-ui, Avenir, Helvetica, Arial, sans-serif;
    margin-bottom: 10px;
    font-size: larger;
}
@keyframes slideIn {
    0% {
        visibility: hidden;
        transform: translateY(5%);
        opacity: 0;
    }
    100% {
        visibility: visible;
        transform: translateY(0);
    }
}

.gradIn {
    animation-duration: 0.25s; /* the duration of the animation */
    animation-timing-function: ease-out; /* how the animation will behave */
    animation-delay: 0s; /* how long to delay the animation from starting */
    animation-iteration-count: 1; /* how many times the animation will play */
    animation-name: slideIn; /* the name of the animation we defined above */
}

.hidden{
    visibility: hidden;
}

</style>
