<template>
  <div class="card">
    <h1>Kristina Kalbasuik</h1>
    <h2>Data Scientist</h2>

    <div class="card-icons">
      <a href="mailto:k.kalbasuik@gmail.com">
        <fa icon="envelope" class="card-icon" />
      </a>

      <a href="https://github.com/kkalbasiuk">
        <fa :icon="['fab', 'github']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc" class="hide">
        <fa :icon="['fab', 'twitter']" class="card-icon" />
      </a>

      <a href="https://www.linkedin.com/in/kristina-kalbasiuk">
        <fa :icon="['fab', 'linkedin']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc" class="hide">
        <fa :icon="['fab', 'medium']" class="card-icon" />
      </a>

      <a href="skype:live:a796f42f22545dbf?chat">
        <fa :icon="['fab', 'skype']" class="card-icon" />
      </a>

      <a href="https://t.me/kkkriskk">
        <fa :icon="['fab', 'telegram']" class="card-icon" />
      </a>

      <a href="https://github.com/nlebedevinc" class="hide">
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

.hide {
  display: none;
}

.card-icon {
  font-size: 32px;
  margin: 5px;
}

.card-icons a {
  color: #000;
}

.card-icons a:hover {
  color: #f0be69;
}

</style>
