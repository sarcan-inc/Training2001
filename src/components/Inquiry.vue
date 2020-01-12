<template>
  <section>
    <h2>INQUIRY</h2>
    <form action>
      <table>
        <tr>
          <th>お名前</th>
          <td>
            <input type="text" v-model="inquiry.name">
            <span>{{inquiry.name}}</span>
          </td>
        </tr>
        <tr>
          <th>Email</th>
          <td>
            <input type="text" v-model.lazy="inquiry.mail">
            <span>{{inquiry.mail}}</span>
          </td>
        </tr>
      </table>
      <div>
        <input type="submit" value="確認">
      </div>
    </form>
  </section>
</template>

<script>
export default {
  data() {
    return {
      inquiry: {
        name: "",
        mail: ""
      }
    };
  }
};
</script>
