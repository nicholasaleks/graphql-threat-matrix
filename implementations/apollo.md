# Apollo

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [javascript](https://www.javascript.com/)\
Source: [https://github.com/apollographql/apollo-server](https://github.com/apollographql/apollo-server)\
Documentation: [https://www.apollographql.com/docs/apollo-server/](https://www.apollographql.com/docs/apollo-server/)

## Security Considerations
Apollo provides the following features which should be taken into consideration:

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
		<td align="center">⚠️<br>Disabled by Default (Supported via External Libraries)</td>
		<td align="center">⚠️<br>Disabled by Default (Supported via External Libraries)</td>
		<td align="center">❌<br>No Support</td>
		<td align="center">✅<br>Enabled if NODE_ENV is not set to 'production' </td>
		<td align="center">✅<br>exception.stacktrace exists if NODE_ENV is not set to 'production' or 'test' </td>
		<td align="center">✅<br>Enabled by Default</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **34**

Apollo is based on [graphql-js](https://github.com/graphql/graphql-js) which validates the following checks when a query is sent:

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
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/ExecutableDefinitionsRule.ts">Executable Definitions</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/LoneAnonymousOperationRule.ts">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/FieldsOnCorrectTypeRule.ts">Fields On Correct Type</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/KnownArgumentNamesRule.ts">Known Argument Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/FragmentsOnCompositeTypesRule.ts">Fragments On Composite Types</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/KnownTypeNamesRule.ts">Known Type Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/KnownDirectivesRule.ts">Known Directives</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/NoUndefinedVariablesRule.ts">No Undefined Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/LoneSchemaDefinitionRule.ts">Lone Schema Definition</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueOperationNamesRule.ts">Unique Operation Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/OverlappingFieldsCanBeMergedRule.ts">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/ProvidedRequiredArgumentsRule.ts">Provided Required Arguments</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/KnownFragmentNamesRule.ts">Known Fragment Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/PossibleTypeExtensionsRule.ts">Possible Type Extensions</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueDirectiveNamesRule.ts">Unique Directive Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/NoUnusedVariablesRule.ts">No Unused Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueOperationNamesRule.ts">Unique Operation Types</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/ScalarLeafsRule.ts">Scalar Leafs</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueArgumentDefinitionNamesRule.ts">Unique Argument Definition Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/NoFragmentCyclesRule.ts">No Fragment Cycles</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueEnumValueNamesRule.ts">Unique Enum Value Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueDirectivesPerLocationRule.ts">Unique Directives Per Location</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueVariableNamesRule.ts">Unique Variable Names</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/SingleFieldSubscriptionsRule.ts">Single Field Subscriptions</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueArgumentNamesRule.ts">Unique Argument Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/NoUnusedFragmentsRule.ts">No Unused Fragments</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueTypeNamesRule.ts">Unique Type Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/VariablesAreInputTypesRule.ts">Variables Are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueFieldDefinitionNamesRule.ts">Unique Field Definition Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/PossibleFragmentSpreadsRule.ts">Possible Fragment Spreads</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/ValuesOfCorrectTypeRule.ts">Values Of Correct Type</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/VariablesInAllowedPositionRule.ts">Variables In Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueFragmentNamesRule.ts">Unique Fragment Names</a></td>
		<td><a href="https://github.com/graphql/graphql-js/blob/main/src/validation/rules/UniqueInputFieldNamesRule.ts">Unique Input Field Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>