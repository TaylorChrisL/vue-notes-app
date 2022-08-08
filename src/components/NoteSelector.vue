<script>
export default {
  props: ["potato", "selectedNoteId"],
};
</script>
<template>
  <div class="note-selector" v-bind:class="{ active: selectedNoteId === potato.id }">
    <p class="note-selector-title">{{ potato.body }}</p>
    <p class="note-selector-timestamp">{{ potato.timestamp }}</p>
  </div>
</template>
