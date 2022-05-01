# gqlgen

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [php](https://www.php.net/)\
Source: [https://github.com/99designs/gqlgen](https://github.com/99designs/gqlgen)\
Documentation: 
- [https://gqlgen.com/](https://gqlgen.com/)
- [https://github.com/vektah/gqlparser](https://github.com/vektah/gqlparser)

## Security Considerations
graphql-js provides the following features which should be taken into consideration:

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
		<td align="center">✅<br>Enabled by Default</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">✅<br>Enabled by Default</td>
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">⚠️<br>Disabled by Default</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **25**

gqldwn validates the following checks when a query is sent:

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
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/lone_anonymous_operation.go">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/single_field_subscriptions.go">Single Field Subscriptions</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/fields_on_correct_type.go">Fields on Correct Type</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/known_argument_names.go">Known Argument Names</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/fragments_on_composite_types.go">Fragments on Composite Types</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/known_type_names.go">Known Type Names</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/known_directives.go">Known Directives</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/no_undefined_variables.go">No Undefined Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/unique_operation_names.go">Unique Operation Names</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/overlapping_fields_can_be_merged.go">Overlapping Fields can be Merged</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/provided_required_arguments.go">Provided Required Arguments</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/known_fragment_names.go">Known Fragment Names</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/unique_input_field_names.go">Unique Input Field Names</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/unique_directives_per_location.go">Unique Directives per Location</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/no_unused_variables.go">No Unused Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/scalar_leafs.go">Scalar Leafs</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/unique_argument_names.go">Unique Argument Names</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/no_fragment_cycles.go">No Fragment Cycles</a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/values_of_correct_type.go">Values of Correct Type</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/unique_variable_names.go">Unique Variable Names</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/no_unused_fragments.go">No Unused Fragments</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/variables_are_input_types.go">Variables are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/possible_fragment_spreads.go">Possible Fragment Spreads</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/variables_in_allowed_position.go">Variables in Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/vektah/gqlparser/blob/master/validator/rules/unique_fragment_names.go">Unique Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>