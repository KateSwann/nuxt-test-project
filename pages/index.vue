<template>
  <section class="container">
    <nuxt-link to="/users">Users</nuxt-link>
    <p id="demo" onclick="myFunction()">Click me to change my text color.</p>

    <div class="yamap" id="ymaps">
        <script type="text/javascript" charset="utf-8" async src="https://api-maps.yandex.ru/services/constructor/1.0/js/?um=constructor%3A519cec2f984af94a5183fc2b7ccb23aee7b2531f0183ea0056f6719289446201&amp;width=100%&amp;lang=ru_RU&amp;scroll=true"></script>
    </div>
  </section>
</template>


<script>
function myFunction() {
    document.getElementById("demo").style.color = "red";
}
</script>


<style>
.yamap {
  height: 80vh;
}

.container {
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
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
</style>

