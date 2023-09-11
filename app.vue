<template>
  <nav>
    <ul>
      <li>
        <NuxtLink to="/hydration-mismatch">
          Hydration Mismatch
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/fat-payload">
          Fat Payload
        </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/pre-hydration">
          Pre Hydration
        </NuxtLink>
      </li>
    </ul>
  </nav>
  <NuxtPage />
</template>

<style>
nav {
  width: 100%;
  background: #fff;
  padding: 1rem;
  box-shadow: 0 0 1rem rgba(0, 0, 0, 0.1);
}

nav ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

nav ul li {
  margin-right: 1rem;
}
</style>