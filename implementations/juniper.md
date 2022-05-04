# juniper

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)
* [Notable Vulnerabilities](#Notable-Vulnerabilties)
* [Security Disclosure](#Security-Disclosure)

## About
Language: [rust](https://www.rust-lang.org/)\
Source: [https://github.com/graphql-rust/juniper](https://github.com/graphql-rust/juniper)\
Documentation: [https://graphql-rust.github.io/](https://graphql-rust.github.io/)

## Security Considerations
juniper provides the following features which should be taken into consideration:

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
		<td align="center">⚠️<br>Disabled by Default</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **24**

juniper validates the following checks when a query is sent:

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
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/lone_anonymous_operation.rs">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/fields_on_correct_type.rs">Fields on Correct Type</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/arguments_of_correct_type.rs">Arguments of Correct Type</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/fragments_on_composite_types.rs">Fragments on Composite Types</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/default_values_of_correct_type.rs">Default Values of Correct Type</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/known_directives.rs">Known Directives</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/no_undefined_variables.rs">No Undefined Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/unique_operation_names.rs">Unique Operation Names</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/overlapping_fields_can_be_merged.rs">Overlapping Fields can be Merged/a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/known_argument_names.rs">Known Argument Names</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/known_fragment_names.rs">Known Fragment Names</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/known_type_names.rs">Known Type Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/no_unused_variables.rs">No Unused Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/scalar_leafs.rs">Scalar Leafs</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/provided_non_null_arguments.rs">Provided non null arguments</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/no_fragment_cycles.rs">No Fragment Cycles</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/unique_variable_names.rs">Unique Variable Names</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/unique_input_field_names.rs">Unique Input Field Names</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/unique_argument_names.rs">Unique Argument Names</a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/no_unused_fragments.rs">No Unused Fragments</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/variables_are_input_types.rs">Variables are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/possible_fragment_spreads.rs">Possible Fragment Spreads</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/variables_in_allowed_position.rs">Variables in Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-rust/juniper/blob/master/juniper/src/validation/rules/unique_fragment_names.rs">Unique Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>

## Security Disclosure
https://github.com/graphql-rust/juniper/issues