<template>
  <header>
    <h1>Vue Training</h1>
    <p>Sarcan inc.</p>
    <slot></slot>
  </header>
</template>

<style>
header {
  text-align: center;
}
header nav ul li {
  display: inline;
  padding: 5px 20px;
}
</style>
