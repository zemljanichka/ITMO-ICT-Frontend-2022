<template>
  <div class="d-flex events" :id="itemId">
    <img class="search-image m-1" :src="imgUrl" alt="event" />
    <div
      style="width: 100%"
      class="d-flex flex-column justify-content-evenly ms-2"
    >
      <span style="color: gray" class="fw-bold"> {{ test }}</span>
      <span style="color: black" class="fw-bold"> {{ name }} </span>
      <span style="color: rgb(104, 91, 91)" class="fw-light">
        {{ type }} . {{ city }}, {{ country }}</span
      >
      <div class="d-flex justify-content-between search-result-description">
        <span style="color: rgb(104, 91, 91)" class="fw-light"
          > {{ eventId }} attendees</span
        >
        <svg
          style="color: rgb(104, 91, 91); margin-right: 10px"
          xmlns="http://www.w3.org/2000/svg"
          width="16"
          height="16"
          fill="currentColor"
          class="bi bi-box-arrow-up"
          viewBox="0 0 16 16"
        >
          <path
            fill-rule="evenodd"
            d="M3.5 6a.5.5 0 0 0-.5.5v8a.5.5 0 0 0 .5.5h9a.5.5 0 0 0 .5-.5v-8a.5.5 0 0 0-.5-.5h-2a.5.5 0 0 1 0-1h2A1.5 1.5 0 0 1 14 6.5v8a1.5 1.5 0 0 1-1.5 1.5h-9A1.5 1.5 0 0 1 2 14.5v-8A1.5 1.5 0 0 1 3.5 5h2a.5.5 0 0 1 0 1h-2z"
          />
          <path
            fill-rule="evenodd"
            d="M7.646.146a.5.5 0 0 1 .708 0l3 3a.5.5 0 0 1-.708.708L8.5 1.707V10.5a.5.5 0 0 1-1 0V1.707L5.354 3.854a.5.5 0 1 1-.708-.708l3-3z"
          />
        </svg>
      </div>
    </div>
  </div>
  <hr />
</template>

<script>
export default {
  name: "EventItem",
  props: {
    imgUrl: String,
    itemId: Number,
    eventId: Number,
    test: String,
    type: String,
    city: String,
    country: String,
    name: String,
  },
};
</script>

<style>
</style>