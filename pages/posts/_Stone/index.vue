<template>
  <div class="d1">
    <div class="d3">
      <h1>Title</h1>
      <h3>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer arcu
        purus, scelerisque eget eros eget, tempor pharetra urna. Nulla facilisi.
        Mauris molestie felis at arcu semper porttitor. Proin egestas quis
        sapien vitae malesuada. Ut semper urna et leo ornare pellentesque eget
        eu quam. Nam non venenatis orci, ac interdum urna. Pellentesque
        bibendum, lectus porttitor iaculis pulvinar, felis leo vestibulum arcu,
        sed malesuada risus risus sit amet mauris
      </h3>
    </div>
    <div class="d2">
      <img src="~/assets/pic.jpg" alt="stone" />
      <table>
        <tr>
          <th>Name</th>
          <th>Grade</th>
          <th>Size</th>
          <th>Surface</th>
          <th>Price</th>
        </tr>
        <tr>
          <td>Some 1</td>
          <td>A</td>
          <td>40 * 40</td>
          <td>some3 some 3</td>
          <td>450$</td>
        </tr>
      </table>
      <div class="d3">
        <h3>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer arcu
          purus, scelerisque eget eros eget, tempor pharetra urna. Nulla
          facilisi.<br /><br />
          Mauris molestie felis at arcu semper porttitor. Proin egestas quis
          sapien vitae malesuada. Ut semper urna et leo ornare pellentesque eget
          eu quam. Nam non venenatis orci, ac interdum urna. Pellentesque
          bibendum, lectus porttitor iaculis pulvinar, felis leo vestibulum
          arcu, sed malesuada risus risus sit amet mauris
        </h3>
      </div>
    </div>
  </div>
</template>

<style scoped>
.d1 {
  margin-top: 3em;
}
.d3 {
  margin: 0 0 2em 4em;
}
.d2 {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
img {
  max-width: 80%;
  margin: 3em auto;
  height: auto;
}
table {
  margin-top: 2em;
}
h3 {
  font-weight: lighter;
}
table {
  border-collapse: collapse;
  margin-bottom: 3em;
}
td,
th {
  padding: 1em;
  border: 0.5px var(--sixth) solid;
  text-align: center;
}
</style>
