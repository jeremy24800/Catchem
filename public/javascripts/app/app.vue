<template lang="jade">
#logo Catchem
#slogan Buy APPs at the right time
header
  nav
    a(v-link="{ name: 'apps', exact: true }") APPS
    a(v-link="{ name: 'integrations', exact: true }") INTEGRATIONS
router-view
</template>

<script>

</script>

<style>
@import "normalize.css";
@import "purecss";
@import "../../../node_modules/nprogress/nprogress.css";

body{
  color: #555459;
  width: 960px;
  margin: 0 auto;
  margin-top: 4em;
  font-family: 'Source Sans Pro', 'Helvetica Neue', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
}

input{
  outline: none;
}

.v-link-active{
  border-bottom-color: #000;
}

#logo{
  text-align: center;
  font-size: 4em;
  font-weight: lighter;
}

#slogan{
  text-align: center;
  margin: .4em;
  font-size: .8em;
}

header{
  margin-top: 2em;
  nav{
    text-align: center;

    a{
      transition: all .2s;
      margin: 1em;
      padding-bottom: .4em;
      color: #000;
      text-decoration: none;
      border-bottom: 2px solid #fff;
      &:hover{
        border-bottom-color: #000;
      }
    }
  }
}
</style>
