<template>
  <div id="app">
    <table>
      <tr class="header">
        <td>html</td>
        <td></td>
        <td>variable value</td>
        <td>variable name</td>
      </tr>
      <tr>
        <td><label>Type any text : </label><input type="text" v-model="myText"/></td>
        <td>=></td>
        <td>{{myText}}</td>
        <td>myText</td>
      </tr>
      <tr>
        <td><label for="myCheckbox">Check the checkbox : </label><input type="checkbox" v-model="myCheckbox"/></td>
        <td>=></td>
        <td>{{myCheckbox}}</td>
        <td>myCheckbox</td>
      </tr>
      <tr>
        <td><label for="myDate">Choose a date : </label><input type="date" v-model="myDate"/></td>
        <td>=></td>
        <td>{{myDate}}</td>
        <td>myDate</td>
      </tr>
      <tr>
        <td>
          <label>Tick a radio button : </label>
          <input type="radio" name="myRBGroup" id="rb1" v-model="myRB" value="RB1"/><label for="rb1">Radio button 1</label>
          <input type="radio" name="myRBGroup" id="rb2" v-model="myRB" value="RB2"/><label for="rb2">Radio button 2</label>
        </td>
        <td>=></td>
        <td>{{myRB}}</td>
        <td>myRB</td>
      </tr>
      <tr>
        <td>
          <label>Select one option for select number 1 : </label>
          <select v-model="selectSingle">
            <option value="option1_1">option1_1</option>
            <option value="option1_2">option1_2</option>
            <option value="option1_3">option1_3</option>
            <option value="option1_4">option1_4</option>
          </select>
        </td>
        <td>=></td>
        <td>{{selectSingle}}</td>
        <td>selectSingle</td>
      </tr>
      <tr>
        <td>
          <label>Select one or several options for select number 2 : </label>
          <select multiple v-model="selectMultiple">
            <option value="option2_1">option2_1</option>
            <option value="option2_2">option2_2</option>
            <option value="option2_3">option2_3</option>
            <option value="option2_4">option2_4</option>
          </select>
        </td>
        <td>=></td>
        <td>{{selectMultiple}}</td>
        <td>selectMultiple</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: 'app',
  data: function () {
    return {
      myText: '',
      myCheckbox: false,
      myDate: null,
      myRB: null,
      selectSingle: null,
      selectMultiple: []
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

table {
  border:none;
  margin-left:auto;
  margin-right:auto;
}

.header {
  font-weight:bold;
}
</style>
