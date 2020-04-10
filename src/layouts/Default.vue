<template>
  <main class="layout" role="main">
    <slot />
    <div class="footer">
      <p>
        <!-- hitwebcounter Code START -->

        <img
          src="https://hitwebcounter.com/counter/counter.php?page=7227308&style=0038&nbdigits=3&type=page&initCount=0"
          title="Visitor Count"
          alt="Hits"
          border="0"
        />

        <br />Made with ⌛️ by
        <a
          class="link"
          href="https://www.linkedin.com/in/tarundhamor/"
          target="_blank"
        >Tarun Dhamor</a>
      </p>
    </div>
  </main>
</template>

<style>
body {
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
  border: 7px solid #00ffa5;
  min-height: 100vh;
  background-color: #000000;
  color: #ffffff;
}

.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.footer {
  padding-top: calc(30em / 4);
  text-align: center;
  font-size: 1em;
}

.link {
  border: 0px solid #00ffa5;
  padding: 3px;
  color: #00ffa5;
  text-decoration: underline;
}
</style>
