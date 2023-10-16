<script lang="ts">
  export let href: string
  export let text: string
  export let title: string
</script>

<li id="item" {title}>
  <a id="link" {href}>{text}</a>
</li>

<style>
  #item {
    list-style: none;
  }

  #link {
    position: relative;

    text-decoration: none;
    color: #000;
  }

  #link::after {
    content: '';

    position: absolute;
    bottom: -0.1rem;
    left: 0;

    width: 0;
    height: 1px;

    background-color: #000;
    transition: width 0.2s ease-in-out;
  }

  #link:hover::after {
    width: 100%;
  }
</style>
