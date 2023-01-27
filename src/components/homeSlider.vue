<template>
  <section class="slider">
    <div class="slider__wrapper">
      <div class="container">
        <div class="row slider__inner">
          <div class="col-50">
            <div class="slider__title">
              Грузоперевозки по Краснодару и Краснодарскому краю
            </div>
          </div>
          <div class="col-50"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../styles/_variables.scss";

.slider {
  height: 700px;
  background: url("../assets/header.jpg") no-repeat;
  background-size: 100% auto;
  background-position: center;
  &__wrapper {
    background: rgba($green, 0.9);
    width: 100%;
    height: 100%;
  }
  .container {
    height: 100%;
  }
  &__inner {
    height: 100%;
    align-items: center;
  }
  &__title {
    font-size: 64px;
    height: 100%;
    color: #fff;
  }
}
</style>
