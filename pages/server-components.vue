<template>
  <div>
    <h1>Server component</h1>
    <p>This component won't be hydrated. <code>date-fns</code> won't be included in the client-side bundle.</p>
    <div class="box">
      <HeavyComponent />
    </div>
  </div>
</template>

<style>
.box {
  border: 1px solid #ccc;
  padding: 1rem;
}
</style>