<script lang="ts">
  import Logo from './logo.svelte'
</script>

<header id="header">
  <Logo />
  <div id="navigation-container">...</div>
</header>

<style>
  #header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 3.5rem;
    width: 100%;
    background-color: #eee;
    padding: 1rem;
  }
</style>
