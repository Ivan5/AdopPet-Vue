<template>
  <div class="home">
    <h1>Adop a new Best Friend</h1>
    <button class="btn btn-primary">Add New Pet</button>

    <b-form @submit="handleSubmit" v-if="petForm">
      <b-form-group id label="Pets Name" label-for description>
        <b-form-input id type="text" required placeholder/>
      </b-form-group>
    </b-form>
  </div>
</template>

<script>
import { mapActions } from "vuex";
export default {
  name: "home",
  data() {
    return {
      petForm: false
    };
  },
  methods: {
    tooglePetForm() {
      this.petForm = !this.petForm;
    },
    handleSubmit() {}
  }
};
</script>
