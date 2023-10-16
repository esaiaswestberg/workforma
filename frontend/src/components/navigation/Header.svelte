<script lang="ts">
  import Logo from '$components/navigation/Logo.svelte'
  import Navigation from '$components/navigation/Navigation.svelte'
</script>

<header id="header">
  <Logo />
  <Navigation />
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
