<template>
  <div class="home">
    <div class="columns">
      <div class="column is-three-fifths is-offset-one-fifth">
        <transition appear appear-active-class="fade-enter-active">
          <div class="home__content">
            <h1 class="title home__title">Привет! Меня зовут Горовой Иван - я Front-End разработчик.</h1>
            <div
              class="subtitle home__text"
            >Я программист самоучка, увлечённый современными технологиями и обожаю узнавать новое. Верю, что хороший разработчик - это постоянное обучение, сложные проекты и работа над обратной свзяью, что бы стать ещё лучше.</div>
            <button class="button is-primary" @click="$router.push({name: 'projects'})">Мои работы</button>
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
<style scoped>
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

@keyframes go {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
