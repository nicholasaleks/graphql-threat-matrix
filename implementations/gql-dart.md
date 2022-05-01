# gql-dart/gql

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [dart](https://dart.dev/)\
Source: [https://github.com/gql-dart/gql](https://github.com/gql-dart/gql)\

## Security Considerations
gql-dart/gql provides the following features which should be taken into consideration:

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
		<td align="center">❌<br>No Support</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">✅<br>Enabled by Default</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">❌<br>No Support</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **9**

gql-dart/gql validates the following checks when a query is sent:

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
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/lone_schema_definition.dart">Lone Schema Definition</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_field_definition_names.dart">Unique Field Definition Names</a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_argument_names.dart">Unique Argument Names</a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/missing_fragment_definitions.dart">Missing Fragment Definitions</a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_operation_types.dart">Unique Operation Types</a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_directive_names.dart">Unique Directive Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_input_field_names.dart">Unique Input Field Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_type_names.dart">Unique Type Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/gql-dart/gql/blob/master/gql/lib/src/validation/rules/unique_enum_value_names.dart">Unique Enum Value Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>