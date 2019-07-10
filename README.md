# Bind html inputs elements to a variable of a component
For those html elements :
<br/>
input text
<br/>
input checkbox
<br/>
input date
<br/>
input radio
<br/>
select single
<br/>
select multiple
<br/>
<br/>

input text :
<br/>
html&nbsp;=>&nbsp;&nbsp;&nbsp;``<input type="text" v-model="myText"/>``
<br/>
js&nbsp;&nbsp;&nbsp;=>&nbsp;&nbsp;&nbsp;myText: ''
<br/>
<br/>

input checkbox :
<br/>
html =>&nbsp;&nbsp;&nbsp;``<input type="text" v-model="myCheckbox"/>``
<br/>
js&nbsp;&nbsp;&nbsp;=>&nbsp;&nbsp;&nbsp;myCheckbox: false
<br/>
<br/>

input date :
<br/>
html =>&nbsp;&nbsp;&nbsp;``<input type="date" v-model="myDate"/>``
<br/>
js&nbsp;&nbsp;&nbsp;=>&nbsp;&nbsp;&nbsp;myDate: null
<br/>
<br/>

input radio :
<br/>
html =>
<br/>
``<input type="radio" name="myRBGroup" id="rb1" v-model="myRB" value="RB1"/>``
<br/>
``<input type="radio" name="myRBGroup" id="rb2" v-model="myRB" value="RB2"//>``
<br/>
js&nbsp;&nbsp;&nbsp;=>&nbsp;&nbsp;&nbsp;myRB: null
<br/>
<br/>

single select :
<br/>
html =>
<br/>
``<select v-model="selectSingle">``
<br/>
``  <option value="option1_1">option1_1</option>``
<br/>
``  <option value="option1_2">option1_2</option>``
<br/>
``  <option value="option1_3">option1_3</option>``
<br/>
``  <option value="option1_4">option1_4</option>``
<br/>
``</select>``
<br/>
js&nbsp;&nbsp;&nbsp;=>&nbsp;&nbsp;&nbsp;selectSingle: null,
<br/>
<br/>

multiple select :
<br/>
html =>
<br/>
``<select multiple v-model="selectMultiple">``
<br/>
``  <option value="option2_1">option2_1</option>``
<br/>
``  <option value="option2_2">option2_2</option>``
<br/>
``  <option value="option2_3">option2_3</option>``
<br/>
``  <option value="option2_4">option2_4</option>``
<br/>
``</select>``
<br/>
js&nbsp;&nbsp;&nbsp;=>&nbsp;&nbsp;&nbsp;selectMultiple: []
<br/>
<br/>



<style>
.code.html {
  background-color:f8f8fa
  border-radius:5px
}
</style>