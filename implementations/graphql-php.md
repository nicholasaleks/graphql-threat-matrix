# graphql-php

### Table of Contents
* [About](#About)
* [Security Features](#Security-Features)
* [Validations](#Validations)

## About
Language: [php](https://www.php.net/)\
Source: [https://github.com/webonyx/graphql-php](https://github.com/webonyx/graphql-php)\
Documentation: [https://webonyx.github.io/graphql-php/](https://webonyx.github.io/graphql-php/)

## Security Features
GraphQL PHP provides the following features which should be taken into consideration:

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
		<td align="center">⚠️<br>Disabled by Default</td>
	</tr>
</table>

## Validations
Total Validation Count: **37**

GraphQL Ruby validates the following checks when a query is sent:

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
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/ExecutableDefinitions.php">Executable Definitions</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/LoneAnonymousOperation.php">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/FieldsOnCorrectType.php">Fields on Correct Type</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/KnownArgumentNames.php">Known Argument Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/FragmentsOnCompositeTypes.php">Fragments On Composite Types</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/KnownTypeNames.php">Known Type Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/KnownDirectives.php">Known Directives</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/NoUndefinedVariables.php">No Undefined Variables</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/QueryComplexity.php">Query Complexity</a></td>
	</tr>
	<tr>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/LoneSchemaDefinition.php">Lone Schema Definition</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueOperationNames.php">Unique Operation Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/OverlappingFieldsCanBeMerged.php">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/KnownArgumentNamesOnDirectives.php">Known Argument Names On Directives</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/KnownFragmentNames.php">Known Fragment Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/PossibleTypeExtensions.php">Possible Type Extensions</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueDirectiveNames.php">Unique Directive Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/NoUnusedVariables.php">No Unused Variables</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/QueryDepth.php">Query Depth</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/ScalarLeafs.php">Scalar Leafs</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/ProvidedRequiredArguments.php">Provided Required Arguments</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/NoFragmentCycles.php">No Fragment Cycles</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueEnumValueNames.php">Unique Enum Value Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueDirectivesPerLocation.php">Unique Directives Per Location</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueVariableNames.php">Unique Variable Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/DisableIntrospection.php">Disable Introspection</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/SingleFieldSubscription.php">Single Field Subscription</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueArgumentNames.php">Unique Argument Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/NoUnusedFragments.php">No Unused Fragments</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueOperationTypes.php">Unique Operation Types</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/VariablesAreInputTypes.php">Variables Are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueInputFieldNames.php">Unique Input Field Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/ProvidedRequiredArgumentsOnDirectives.php">Provided Required Arguments On Directives</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/PossibleFragmentSpreads.php">Possible Fragment Spreads</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueTypeNames.php">Unique Type Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/VariablesInAllowedPosition.php">Variables In Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/UniqueFragmentNames.php">Unique Fragment Names</a></td>
		<td><a href="https://github.com/webonyx/graphql-php/blob/master/src/Validator/Rules/ValuesOfCorrectType.php">Values Of Correct Type</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>