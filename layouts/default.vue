<template>
  <div>
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Cormorant', serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

button,
textarea {
  font-family: 'Cormorant', serif;
  border: 1px solid transparent;
  outline: none;
}

input {
  border: 1px solid transparent;
  outline: none;
}

textarea:active,
textarea:hover,
textarea:focus,
input:active,
input:hover,
input:focus {
  border: 1px solid #e8e0da;
}

button:active,
button:hover,
button:focus {
  background: #fbf9f8;
  border: 1px solid #e8e0da;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.thin {
  font-weight: 300;
}

.italic {
  font-style: italic;
}
</style>
