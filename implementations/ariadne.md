# ariadne

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [python](https://www.python.org/)\
Source:
- [https://github.com/mirumee/ariadne](https://github.com/mirumee/ariadne)
- [https://github.com/graphql-python/graphql-core](https://github.com/graphql-python/graphql-core)

Documentation: [https://ariadnegraphql.org/](https://ariadnegraphql.org/)

## Security Considerations
ariadne provides the following features which should be taken into consideration:

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
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">✅<br>Enabled by Default</td>
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">❌<br>No Support</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **34**

ariadne is based on [graphql-core](https://github.com/graphql-python/graphql-core) which validates the following checks when a query is sent:

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
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/executable_definitions.py">Executable Definitions</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/lone_anonymous_operation.py">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/fields_on_correct_type.py">Fields On Correct Type</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/known_argument_names.py">Known Argument Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/fragments_on_composite_types.py">Fragments On Composite Types</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/known_type_names.py">Known Type Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/known_directives.py">Known Directives</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/no_undefined_variables.py">No Undefined Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/lone_schema_definition.py">Lone Schema Definition</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_operation_names.py">Unique Operation Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/overlapping_fields_can_be_merged.py">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/provided_required_arguments.py">Provided Required Arguments</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/known_fragment_names.py">Known Fragment Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/possible_type_extensions.py">Possible Type Extensions</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_directive_names.py">Unique Directive Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/no_unused_variables.py">No Unused Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/scalar_leafs.py">Scalar Leafs</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_argument_definition_names.py">Unique Argument Definition Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/no_fragment_cycles.py">No Fragment Cycles</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_enum_value_names.py">Unique Enum Value Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_directives_per_location.py">Unique Directives Per Location</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_variable_names.py">Unique Variable Names</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/single_field_subscriptions.py">Single Field Subscriptions</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_argument_names.py">Unique Argument Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/no_unused_fragments.py">No Unused Fragments</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_operation_types.py">Unique Operation Types</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/variables_are_input_types.py">Variables Are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_field_definition_names.py">Unique Field Definition Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/possible_fragment_spreads.py">Possible Fragment Spreads</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_type_names.py">Unique Type Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/variables_in_allowed_position.py">Variables In Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_input_field_names.py">Unique Input Field Names</a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/unique_fragment_names.py">Unique Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-python/graphql-core/blob/main/src/graphql/validation/rules/values_of_correct_type.py">Values Of Correct Type</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>