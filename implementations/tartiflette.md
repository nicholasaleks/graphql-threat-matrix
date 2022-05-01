# tartiflette

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [https://www.python.org/](https://www.python.org/)\
Source: [https://github.com/tartiflette/tartiflette](https://github.com/tartiflette/tartiflette)\
Documentation: [https://tartiflette.io/](https://tartiflette.io/)

## Security Considerations
Tartiflette provides the following features which should be taken into consideration:

<table>
	<tr>
		<th align="center">Field Suggestions</th>
		<th align="center">Query Depth Limit</th>
		<th align="center">Query Cost Analysis</th>
		<th align="center">Automatic Persisted Queries</th>
		<th align="center">Introspection</th>
		<th align="center">Debug Mode</th>
		<th align="center">Batch Requests</th>
	</tr>
	<tr>
		<td align="center">❌<br>No Support</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">✅<br>Enabled by Default</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">❌<br>No Support</td>
	</tr>
</table>

*Despite Tartiflette not having basic security support, it does provide rate limits on a per field basis.*

## Request Validations
Total Validation Count: **26**

<table>
	<tr>
		<th><a href="https://spec.graphql.org/October2021/#sec-Documents">Document Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Validation.Operations">Operation Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Validation.Fields">Field Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Validation.Arguments">Argument Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Validation.Fragments">Fragment Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Values">Value Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Validation.Directives">Directive Validations</a></th>
		<th><a href="https://spec.graphql.org/October2021/#sec-Validation.Variables">Variable Validations</a></th>
		<th>Misc. Validations</th>
	</tr>
	<tr>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/single_root_field.py">Single Root Field</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/lone_anonymous_operation.py">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/field_selections_on_objects_interfaces_and_unions_types.py">Field Selections on Objects Interfaces and Unions Types</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/argument_names.py">Argument Names</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragment_must_be_used.py">Fragment Must be Used</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/values_of_correct_type.py">Values of Correct Type</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/directives_are_defined.py">Directives are Defined</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/all_variable_usages_are_allowed.py">All Variable Usages are Allowed</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/executable_definitions.py">Executable Definitions</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/operation_name_uniqueness.py">Operation Name Uniqueness</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/input_object_field_uniqueness.py">Input Object Field Uniqueness</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/argument_uniqueness.py">Argument Uniqueness</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragment_name_uniqueness.py">Fragment Name Uniqueness</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/directives_are_in_valid_locations.py">Directives are in Valid Locations</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/all_variable_uses_defined.py">All Variable uses Defined</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/leaf_field_selections.py">Leaf Field Selections</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/required_arguments.py">Required Arguments</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragment_spread_is_possible.py">Fragment Spread is Possible</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/directives_are_unique_per_location.py">Directives are Unique per Location</a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/all_variables_used.py">All Variables Used</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragment_spread_target_defined.py">Fragment Spread Target Defined</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/variable_uniqueness.py">Variable Uniqueness</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragment_spread_type_existence.py">Fragment Spread Type Existence</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/variables_are_input_types.py">Variables are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragment_spreads_must_not_form_cycles.py">Fragment Spreads Must Not Form Cycles</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/tartiflette/tartiflette/blob/master/tartiflette/language/validators/query/fragments_on_composite_types.py">Fragments on Composite Types</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>