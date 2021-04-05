<template>
  <nav :class="$style.nav">
    <img src="~/assets/images/geekait2.png" alt="logo2" srcset="" :class="$style.logo">
  </nav>
</template>

<script>
export default {
  props: {

  },
};
</script>

<style lang="scss">
@import '~/assets/css/utilities/_variables.scss';

</style>

<style lang="scss" module>
@import '~/assets/css/utilities/_variables.scss';

.logo{
  width:26em;
  height:5em;
  @media (max-width: 520px){
  max-width: 60%;
  max-height: 60%;
  }
}

.nav {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 5;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 6rem;
  padding: 0 5.5rem;
  background-color:rgba(0, 0, 0, 0.7);
  @media (max-width: 520px){
    height:5rem;
  }
}

.text {
  margin: 0;
  overflow: hidden;
  font-size: 3rem;
  text-overflow: ellipsis;
  white-space: nowrap;
}

</style>
