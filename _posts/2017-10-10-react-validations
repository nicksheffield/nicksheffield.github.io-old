---
title: React Validations
---

## Validators

- required
	- options:
		- name       {String}  [Optional] The name of the field. For displaying in error messages. If omitted, the field key will be used

- numeric
	- options:
		- name       {String}  [Optional] The name of the field. For displaying in error messages. If omitted, the field key will be used
		- allowBlank {Boolean} [Optional] defaults to true. If true, don't validate if there is no input

- length
	- options:
		- name       {String}  [Optional] The name of the field. For displaying in error messages. If omitted, the field key will be used
		- allowBlank {Boolean} [Optional] defaults to true. If true, don't validate if there is no input
		- min        {Number}  [Optional] defaults to null. If set, input must be at least this long
		- max        {Number}  [Optional] defaults to null. If set, input must be at most this long

- format
	- options:
		- name       {String}  [Optional] The name of the field. For displaying in error messages. If omitted, the field key will be used
		- allowBlank {Boolean} [Optional] defaults to true. If true, don't validate if there is no input
		- format     {Regex}   [Mandatory] A regular expression to match against the input


## this.validations object

- `results`
	- An object containing all validation results. Every field's valid status, dirty status and message are available in here.

	- An example of the format of a validation result:
		```javascript
		{
			name: 'username',
			dirty: false,
			valid: false,
			message: 'Username is required'
		}
		```

- `setContext(context, statePath?)`
	- ???

- `validateField(field)`
	- Validate a specific field and return the result object. This mutates `results`.

- `validateAll()`
	- Validate every field in the form, and return all results. This mutates `results`.

- `isDirty(field)`
	- Returns whether this field has been validated yet.

- `isValid(field?)`
	- If no field key is provided, return whether all fields are valid or not.
	- If a field key is provided, return whether that field is valid or not.
	- This method will always return true for any fields until validate is specifically called on them, whether via `validateField()` or `validateAll()`.
		This is so we don't display error messages when the component has initially loaded, which is bad UX.

- `isInvalid(field?)`
	- Same as `isValid()` but will return the opposite value.

- `message(field?)`
	- If no field key is provided, return an array of error messages for all fields.
	- If a field key is provided, return the error message for that field.
