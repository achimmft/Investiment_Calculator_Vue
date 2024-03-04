<template>
    <header id="header">
        <img src="investment-calculator-logo.png" alt="Investment calculator">
        <h1>Investment Calculator</h1>
    </header>
</template>

<script>
export default {
    name: 'HeaderBlock'

}
</script>

<style>
#header {
    text-align: center;
    margin: 3rem auto;
}

#header img {
  width: 5rem;
  height: 5rem;
  object-fit: contain;
  background-color: transparent;
}

#header h1 {
  font-size: 1.5rem;
}
</style>