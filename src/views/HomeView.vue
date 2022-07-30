<template>
  <div class="events">
    <h1>Events List</h1>
    <EventCard v-for="event in events" :key="event.id" :event="event"/>
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  name: 'HomeView',
  components: {
    EventCard,
  },

  data() {
    return {
      events: [
        {
          id: 222,
          category: 'Category 1',
          title: 'Some Title',
          description: 'Some Description Here.',
          location: 'California',
          date: 'Feb 14, 2022',
          time: '12:00PM',
          petsAllowed: false,
          orgainzer: 'SomeOne',
        },
        {
          id: 223,
          category: 'Category 1',
          title: 'Some Title',
          description: 'Some Description Here.',
          location: 'California',
          date: 'Feb 14, 2022',
          time: '12:00PM',
          petsAllowed: false,
          orgainzer: 'SomeOne',
        },
      ],
    }
  },
}
</script>


<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>