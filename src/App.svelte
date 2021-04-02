<script>
  import { Row, Button, Col } from "sveltestrap";
  export let name;
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
  <div>
    <i class="fa fa-universal-access fa-3x" />
  </div>
</main>

<section class="container">
  <Row>
    <Col>
      <Button color="primary">Look Ma, a Button!</Button>
    </Col>
  </Row>
</section>

<style type="text/scss">
  $my-h1-colour: #3e3e3e;
  $my-text-colour: #aa0000;
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
    color: $my-text-colour;
    i.fa {
      color: rgba(1, 1, 1, 0.1);
    }
  }

  h1 {
    color: $my-h1-colour;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
