<template>
  <div>
    <h1>Oh no!</h1>
    <h3>
      Looks like you're experiencing some network issues. Please click the back
      button and try again.
    </h3>
    <router-link :to="{ name: 'event-list' }">
      Or, go back home
    </router-link>
  </div>
</template>
