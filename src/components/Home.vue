<template>
  <div class="home">
    <div class="columns">
      <div class="column is-three-fifths is-offset-one-fifth">
        <transition appear appear-active-class="fade-enter-active">
          <div class="home__content">
            <h1 class="title home__title">Привет! Меня зовут Горовой Иван - я Front-End разработчик.</h1>
            <div
              class="subtitle home__text"
            >Я программист-самоучка, увлечённый современными технологиями и обожаю узнавать новое. Верю, что хороший разработчик это постоянное обучение, сложные проекты и работа над обратной связью, что бы стать ещё лучше.</div>
            <div class="columns is-mobile">
              <div class="column is-9">
                <button
                  class="button is-primary"
                  @click="$router.push({name: 'projects'})"
                >Мои работы</button>
              </div>
              <div class="column is-3 is-pulled-right">
                <a class="icon is-medium" href="https://github.com/Pupinia" target="_blank">
                  <i class="fab fa-github"></i>
                </a>
                <a class="icon is-medium" href="mailto:ivangorovoyyy@gmail.com" target="_blank">
                  <i class="fas fa-envelope"></i>
                </a>
              </div>
            </div>
          </div>
        </transition>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.home {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100%;
  font-family: "Open Sans";
}
.home__content {
  text-align: left;
}
.home__title {
  margin-bottom: 10px;
  margin-bottom: 35px !important;
  line-height: 45px;
}
.fade-enter-active {
  animation: go 1s;
}

.icon {
  font-size: 1.7em;
  margin: 5px;
  color: #00d1b2;
  &:hover {
    color: #00c4a7;
  }
  @media (max-width: 550px) {
    margin: 2px;
  }
}

@keyframes go {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
