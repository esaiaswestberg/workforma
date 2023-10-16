<script lang="ts">
  import NavigationItem from '$components/navigation/NavigationItem.svelte'
</script>

<ul id="navigation">
  <NavigationItem href="/" text="Home" title="Home page" />
  <NavigationItem href="/dashboard" text="Dashboard" title="Administration dashboard" />
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
