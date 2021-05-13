<template>
  <div class="card">
    <h1>Kristina Kalbasuik</h1>
    <h2>Data Scientist</h2>

    <div class="card-icons">
      <a href="https://github.com/nlebedevinc">
        <fa icon="envelope" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'github']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'twitter']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'linkedin']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'medium']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'skype']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'telegram']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc">
        <fa :icon="['fab', 'instagram']" class="card-icon" />
      </a>
    </div>
  </div>
</template>

<style>
.card {
  background-color: #f3f3f3;
  padding: 50px;
  text-align: center;
  z-index: 2;
}

.card-icons {
  margin-top: 30px;
}

.card-icon {
  font-size: 32px;
  margin: 5px;
}
</style>
