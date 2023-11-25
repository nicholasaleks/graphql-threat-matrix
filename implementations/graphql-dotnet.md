# graphql-dotnet

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)
* [Notable Vulnerabilities](#Notable-Vulnerabilties)
* [Security Disclosure](#Security-Disclosure)

## About
Language: [C#](https://dotnet.microsoft.com/en-us/languages/csharp)\
Source: [https://github.com/graphql-dotnet/graphql-dotnet](https://github.com/graphql-dotnet/graphql-dotnet)\
Documentation: [https://graphql-dotnet.github.io/docs/getting-started/introduction/](https://graphql-dotnet.github.io/docs/getting-started/introduction/)

## Security Considerations
graphql-dotnet provides the following features which should be taken into consideration:

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
		<td align="center">❌<br>No Support</td>
		<td align="center">⚠️<br>Disabled by Default</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **29**

GraphQL.NET validates the following checks when a query is sent:

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
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/LoneAnonymousOperation.cs">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/FieldsOnCorrectType.cs">Fields On Correct Type</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/ArgumentsOfCorrectType.cs">Arguments Of Correct Type</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/FragmentsOnCompositeTypes.cs">Fragments On Composite Types</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/DefaultValuesOfCorrectType.cs">Default Values Of Correct Type</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.7%20-%20Directives/1%2B2.%20KnownDirectivesInAllowedLocations.cs">Known Directives In Allowed Locations</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.8%20-%20Variables/1.%20UniqueVariableNames.cs">Unique Variable Names</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules.Custom/InputFieldsAndArgumentsOfCorrectLength.cs">Input Fields And Arguments Of Correct Length</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/UniqueOperationNames.cs">Unique Operation Names</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/OverlappingFieldsCanBeMerged.cs">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/KnownArgumentNames.cs">Known Argument Names</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/KnownFragmentNames.cs">Known Fragment Names</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/KnownTypeNames.cs">Known Type Names</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.7%20-%20Directives/3.%20UniqueDirectivesPerLocation.cs">Unique Directives Per Location</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.8%20-%20Variables/2.%20VariablesAreInputTypes.cs">Variables Are Input Types</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules.Custom/NoIntrospectionValidationRule.cs">No Introspection Validation Rule</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/ScalarLeafs.cs">Scalar Leafs</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/ProvidedNonNullArguments.cs">Provided Non Null Arguments</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/NoFragmentCycles.cs">No Fragment Cycles</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.8%20-%20Variables/3.%20NoUndefinedVariables.cs">No Undefined Variables</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules.Custom/ComplexityValidationRule.cs">Complexity Validation Rule</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/SingleRootFieldSubscriptions.cs">Single Root Field Subscriptions</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/UniqueArgumentNames.cs">Unique Argument Names</a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/NoUnusedFragments.cs">No Unused Fragments</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.8%20-%20Variables/4.%20NoUnusedVariables.cs">No Unused Variable</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/UniqueInputFieldNames.cs">Unique Input Field Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/PossibleFragmentSpreads.cs">Possible Fragment Spreads</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/5.8%20-%20Variables/5.%20VariablesInAllowedPosition.cs">Variables In Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-dotnet/graphql-dotnet/blob/master/src/GraphQL/Validation/Rules/UniqueFragmentNames.cs">Unique Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>

## Security Disclosure
https://github.com/graphql-dotnet/graphql-dotnet/issues