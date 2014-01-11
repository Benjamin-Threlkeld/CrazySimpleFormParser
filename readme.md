Crazy Simple Form Parser
========

Crazy Simple Form Parser takes this

	options = {
		// first is the index second is the value third is placeholder
		title: ["input", "title test", "Title"],
		// if it is a select then the first index the element second is the selected option and then every other is the option text the next one is the value for that option
		category: ["select", "opt2", "opt1", "val1", "opt2", "val2", "opt3", "val3"],
		location: {
			lat: ["input", "", "Lat"],
			lon: ["input", "", "Lon"]
		}
	}

And creates this

		  <input type="text" name="title" value="title test" placeholder="Title">
	<select name="category">
	  <option value="val1">opt1</option>
	  <option value="val2" selected>opt2</option>
	  <option value="val3">opt3</option>
	</select>
	<div data-parent-name="location">
	  <input type="text" name="lat" value="" placeholder="Lat">
	  <input type="text" name="lon" value="" placeholder="Lon">
	</div>

For now just look at the example until I write how it would be used. Like anyone will actually stumble apon this... and need it :P