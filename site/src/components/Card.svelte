<script>
  export let item
  const { slug, title } = item
</script>

<a href={slug}>
  <h2>{title}</h2>
  <img src="assets/{slug}/{slug}.png" alt={title} />
</a>

<style>
  a {
    display: grid;
    place-content: center;
    border-radius: 1ex;
    transition: 0.5s;
    cursor: pointer;
    transform-style: preserve-3d;
    background: #595975;
    transition: 0.5s;
  }
  a:hover {
    transform: scale(1.02);
  }
  h2 {
    margin: 1ex;
    color: white;
  }
  img {
    box-sizing: border-box;
    width: calc(100% - 2ex);
    background: #ffffff85;
    margin: 1ex;
    padding: 1ex;
    border-radius: 4pt;
  }
</style>
