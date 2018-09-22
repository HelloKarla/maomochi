<template>
  <section>
    <b-field horizontal label="From">
      <b-input name="name" placeholder="Name" expanded></b-input>
      <b-input name="email" type="email" placeholder="nobody@nowhere.com" expanded></b-input>
    </b-field>
    <b-field horizontal label="Topic">
      <b-select placeholder="Select a topic">
          <option value="1">貓貓</option>
          <option value="2">狗狗</option>
      </b-select>
    </b-field>
    <b-field horizontal label="Message">
      <b-input type="textarea"></b-input>
    </b-field>
    <b-field horizontal><!-- Label left empty for spacing -->
      <p class="control">
          <button class="button is-primary">
            Send message
          </button>
      </p>
    </b-field>
  </section>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
