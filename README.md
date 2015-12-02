<pre>
"version": 1,
"questions": 
[
	{
		"question_no": 1,
		"question_text": "Property Type",
		"fields":[
			{
				"name": "property_type"
				"type": "radio",
				"options": [
					{"value": "Apartment", "display": "Apartment"},
					{"value": "Villa", "display": "Villa"},
					{"value": "Independent House", "display": "Independent House"},
				]
			}
		]
	},
		
	{
		"question_no": 2,
		"question_text": "Property Name",
		"fields":[
			{
				"name": "property_name"
				"type": "text",
				"autosuggest": true,
				"api": "http://api.realdocs.com/property/suggest/:propName"
			}
		]
	},

	{
		"question_no": 3,
		"question_text": "Property Address",
		"type": "address",
		"fields":
			{
				"common": [
					{
						"name": "city",
						"type": "text",
						"autosuggest": true,
						"api": "/cities/suggest/:city"
					},
					{
						"name": "region",
						"type": "text",
						"autosuggest": true,
						"api": "/regions/:region/suggest/:city"
					},
					{
						"name": "pincode",
						"type": "text"
					}
				],

				"Apartment": [
					{
						"name": "flat_no"
						"type": "text",
						"placeholder": "Flat No"
					},
					{
						"name": "apartment_name"
						"type": "text",
					},
					
				],

				"Independent House": [
					{
						"name": "flat_no"
						"type": "text",
						"placeholder": "Flat No"
					},
					{
						"name": "line 1"
						"type": "text",
						"placeholder": "Line 1"
					},
					{
						"name": "line 2"
						"type": "text",
						"placeholder": "Line 2"
					}
				],

				"Villa": [
					{
						"name": "flat_no"
						"type": "text",
						"placeholder": "Flat No"
					},
					{
						"name": "line 1"
						"type": "text",
						"placeholder": "Line 1"
					},
					{
						"name": "line 2"
						"type": "text",
						"placeholder": "Line 2"
					}
				]
			}
	},

	{
		"question_no": 4,
		"question_text": "Property Status",
		"fields":[
			{
				"name": "property_status"
				"type": "radio",
				"options": [
					{"value": "UnderConstruction", "display": "UnderConstruction"},
					{"value": "ConstructionComplete", "display": "ConstructionComplete"},
					
				]
			}
		]
	},

	{
		"question_no": 5,
		"question_text": "Loan Status",
		"fields":[
			{
				"name": "loan_status"
				"type": "radio",
				"options": [
					{"value": "NeverTaken", "display": "Never Taken"},
					{"value": "PaidOff", "display": "Paid Off"},
					{"value": "CurrentlyOnLoan", "display": "Currently On Loan"},
					
				]
			}
		]
	},

	{
		"question_no": 6,
		"question_text": "Number of Floors",
		"fields":[
			{
				"name": "number_of_status"
				"type": "radio",
				"options": [
					{"value": "3FloorsOrLesser", "display": "3FloorsOrLesser"},
					{"value": "MoreThan3Floors", "display": "MoreThan3Floors"},
					
					
				]
			}
		]
	},

	{
		"question_no": 7,
		"question_text": "Property Currently Insecured",
		"fields":[
			{
				"name": "property_currently_insecured"
				"type": "radio",
				"options": [
					{"value": "Yes", "display": "Yes"},
					{"value": "No", "display": "No"},
					
					
				]
			}
		]
	},

	

	{
		"question_no": 9,
		"question_text": "Extra Car Park",
		"fields":[
			{
				"name": "extra_car_park"
				"type": "radio",
				"options": [
					{"value": "Yes", "display": "Yes"},
					{"value": "No", "display": "No"},
					
					
				]
			}
		]
	}


		
]
</pre>
