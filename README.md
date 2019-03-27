SelectFilter is a jQuery plugin for creating dependent select boxes where options are derived based on the value selected from other select element(s).

# How to use it:

Link to jQuery library and the jQuery SelectFilter plugin's script
```javascript
<script src="http://code.jquery.com/jquery.min.js"></script>
<script src="selectFilter.min.js"></script>
```
Create select boxes and uses HTML5 data attributes to configure the dependent select options.
```html
<select data-target="secondList" class="firstList selectFilter">
	<option value="-1">Select</option>
	<option data-ref="one" >First One</option>
	<option data-ref="two" >First Two</option>
	<option data-ref="three">First Three</option>
</select>
<br />
<br />
<select data-target="thirdList" class="secondList selectFilter">
	<option value="-1">Select</option>
	<option data-ref="A" data-belong="one" >First One</option>
	<option data-ref="B" data-belong="two">First Two</option>
	<option data-ref="C" data-belong="three">First Three</option>
	<option data-ref="D" data-belong="one">Second One</option>
	<option data-ref="E" data-belong="two">Second Two</option>
	<option data-ref="F" data-belong="three">Second Three</option>
</select>
<br />
<br />
<select class="thirdList selectFilter">
	<option value="-1">Select</option>
	<option data-belong="A" >First One</option>
	<option data-belong="B">First Two</option>
	<option data-belong="C">First Three</option>
	<option data-belong="D">Second One</option>
	<option data-belong="E">Second Two</option>
	<option data-belong="F">Second Three</option>
	<option data-belong="A">Third One</option>
	<option data-belong="B">Third Two</option>
	<option data-belong="C">Third Three</option>

</select>
```
## Note:
- **selectFilter** is a class for select to enable selectFilter plugin.
- **data-target** is use to target class of all select.
- **data-ref** is use to refer the value to filter.
- **data-belong** is use to filter the select by data-ref.

Check the website for **[more information](http://www.tellmehow.co "more information")**.
