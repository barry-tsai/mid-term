<template lang="pug">
  #app
    #nav
      //- router-link(to="/") Home |
      //- router-link(to="/about") About
    router-view
</template>

<style lang="sass">
#app 
  font-family: 華康鋼筆體W2
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50
  background-size: cover
  background-image: url('~@/assets/Background.jpg')
  //position: relative
  background-attachment: fixed

#nav 
  padding: 755px


#nav a 
  font-weight: bold
  color: #2c3e50


#nav a.router-link-exact-active 
  color: #42b983

</style>
