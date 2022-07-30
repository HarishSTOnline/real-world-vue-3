<template>
<div class="event-card">
  <span>@ {{ event.time }} on {{ event.date }}</span>
  <h4>{{ event.title }}</h4>
</div>
</template>

<script>
export default {
  name: 'EventCard',
  props: {
    event: Object
  }
}
</script>

<style scoped>
.event-card {
  padding: 1rem;
  width: 250px;
  cursor: pointer;
  border: 1px solid #ccc;
  margin-bottom: 1rem;
}
</style>
