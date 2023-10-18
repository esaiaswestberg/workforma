<script lang="ts">
  import NavigationItem from '$components/navigation/NavigationItem.svelte'
</script>

<ul id="navigation">
  <NavigationItem href="/app" text="App" title="Workforma dashboard" />
</ul>

<style>
  #navigation {
    display: flex;

    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    gap: 1rem;

    height: 100%;
  }
</style>
