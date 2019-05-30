<template>
  <div class="projects">
    <div class="columns">
      <div class="column">
        <div class="column is-1">
          <button class="button is-link" @click="$router.push({name: 'home'})">Назад</button>
        </div>
      </div>
    </div>
    <div class="columns">
      <div class="column">
        <div class="project">
          <div class="card">
            <div class="card-content">
              <div class="title">Hookah-Mix</div>
              <div class="content">Приложения для хранения рецептов миксов для кальяна</div>
            </div>
            <footer class="card-footer">
              <div class="card-footer-item">
                <a href="https://hookah-mixes-18eb3.firebaseapp.com/" target="_blank">Сайт</a>
              </div>
              <div class="card-footer-item">
                <a href="https://github.com/Pupinia/hookah-mix-app" target="_blank">Репозиторий</a>
              </div>
            </footer>
          </div>
        </div>
      </div>
      <div class="column">
        <div class="project">
          <div class="card">
            <div class="card-content">
              <div class="title">Vue chat</div>
              <div class="content">Чат на vue.js и firebase</div>
            </div>
            <footer class="card-footer">
              <div class="card-footer-item">
                <a href="https://vue-chat-9da3b.firebaseapp.com/" target="_blank">Сайт</a>
              </div>
              <div class="card-footer-item">
                <a href="https://github.com/Pupinia/vue-chat" target="_blank">Репозиторий</a>
              </div>
            </footer>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.projects {
  margin-top: 20px;
}
</style>
