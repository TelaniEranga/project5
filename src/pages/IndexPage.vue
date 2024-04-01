<template>
  <q-page>
    <!-- Hero Section -->
    <q-banner
      class="hero-section"
      style="background-image: url('path_to_your_image.jpg')"
      :dark="true"
    >
      <div class="text-white">
        <h1>Welcome to Our Website</h1>
        <p>Explore our amazing features</p>
      </div>
    </q-banner>

    <!-- Description Section -->
    <div class="q-my-md q-pa-md">
      <h2 class="text-h6">About Us</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi.
      </p>
    </div>

    <!-- Card Section -->
    <div class="q-my-md q-pa-md">
      <h2 class="text-h6">Our Services</h2>
      <q-card
        class="q-my-md"
        v-for="(service, index) in services"
        :key="index"
      >
        <q-card-section>
          <q-item
            clickable
            tag="a"
            :href="service.link"
            class="text-primary"
          >
            <q-item-section>
              <q-item-label>{{ service.title }}</q-item-label>
              <q-item-label caption>{{ service.description }}</q-item-label>
            </q-item-section>
          </q-item>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<script>
export default {
  data () {
    return {
      services: [
        {
          title: 'Service 1',
          description: 'Description of Service 1',
          link: '#'
        },
        {
          title: 'Service 2',
          description: 'Description of Service 2',
          link: '#'
        },
        {
          title: 'Service 3',
          description: 'Description of Service 3',
          link: '#'
        }
      ]
    }
  }
}
</script>

<style scoped>
.hero-section {
  height: 300px;
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.q-my-md {
  margin-top: 20px;
  margin-bottom: 20px;
}

.q-pa-md {
  padding: 20px;
}
</style>
