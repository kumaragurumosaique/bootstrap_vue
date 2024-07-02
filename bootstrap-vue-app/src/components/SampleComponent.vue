<template>
  <div>
    <b-alert show variant="success">
      Hello, BootstrapVue!
    </b-alert>
    <b-container>
      <b-row>
        <b-col>
          <b-card title="Welcome to Vue.js with Bootstrap">
            <p>This is a sample component demonstrating how to integrate Bootstrap with Vue.js.</p>
            <b-button variant="primary" @click="handleClick">Click me</b-button>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
    <b-dropdown id="dropdown-1" text="Dropdown Button" @click="toggleDropdown">
      <b-dropdown-item>Action 1</b-dropdown-item>
      <b-dropdown-item>Action 2</b-dropdown-item>
      <b-dropdown-item>Action 3</b-dropdown-item>
      <b-dropdown-divider></b-dropdown-divider>
      <b-dropdown-item>Action 4</b-dropdown-item>
    </b-dropdown>
    <!-- Bootstrap collapse component -->
    <div class="d-inline-flex gap-1">
      <a class="btn btn-primary" data-bs-toggle="collapse" href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample">
        Link with href
      </a>
      <button class="btn btn-primary" type="button" data-bs-toggle="collapse" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
        Button with data-bs-target
      </button>
    </div>
    <div class="collapse" id="collapseExample">
      <div class="card card-body">
        Some placeholder content for the collapse component. This panel is hidden by default but revealed when the user activates the relevant trigger.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SampleComponent',
  methods: {
    handleClick() {
      console.log("Welcome")
    },
    toggleDropdown() {
      // Implement dropdown toggle functionality if needed
    }
  }
};
</script>

<style scoped>
/* Add any component-specific styles here */
</style>
