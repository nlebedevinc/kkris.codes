<template>
  <div id="index">
    <Particles
      id="tsparticles"
      :options="{
        background: {
          color: {
            value: '#2e2e2e',
          },
        },
        fullScreen: {
          enable: true,
          zIndex: 1,
        },
        interactivity: {
          events: {
            onClick: {
              enable: true,
              mode: 'push',
            },
            onHover: {
              enable: true,
              mode: 'grab',
            },
          },
        },
        particles: {
          color: {
            value: '#ff0000',
            animation: {
              h: {
                enable: true,
                speed: 20,
              },
            },
          },
          links: {
            color: {
              value: '#ffffff',
            },
            enable: true,
            opacity: 0.4,
          },
          move: {
            enable: true,
            path: {},
            outModes: {
              bottom: 'out',
              left: 'out',
              right: 'out',
              top: 'out',
            },
          },
          number: {
            density: {
              enable: true,
            },
            value: 80,
          },
          opacity: {
            value: 0.5,
            animation: {
              speed: 4,
            },
          },
          size: {
            value: {
              min: 0.5,
              max: 4,
            },
            animation: {
              speed: 1,
            },
          },
          twinkle: {
            lines: {
              frequency: 0.1,
            },
          },
        },
      }"
    />
    <Card />
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({});
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

#index {
  background-color: #222;
  height: 100vh;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

#tsparticles {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}
</style>
