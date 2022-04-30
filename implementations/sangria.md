# Sangria

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [Scala](https://www.scala-lang.org/)\
Source: [https://github.com/sangria-graphql/sangria](https://github.com/sangria-graphql/sangria)\
Documentation: [https://sangria-graphql.github.io/learn/](https://sangria-graphql.github.io/learn/)\

## Security Considerations
GraphQL Sangria provides the following features which should be taken into consideration:

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
Total Validation Count: **27**

GraphQL Sangria validates the following checks when a query is sent:

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
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/ExecutableDefinitions.scala">Executable Definitions</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/LoneAnonymousOperation.scala">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/FieldsOnCorrectType.scala">Fields On Correct Type</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/KnownArgumentNames.scala">Known Argument Names</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/FragmentsOnCompositeTypes.scala">Fragments On Composite Types</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/KnownTypeNames.scala">Known Type Names</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/KnownDirectives.scala">Known Directives</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/InputDocumentNonConflictingVariableInference.scala">Input Document Non Conflicting Variable Inference</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/UniqueOperationNames.scala">Unique Operation Names</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/OverlappingFieldsCanBeMerged.scala">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/ProvidedRequiredArguments.scala">Provided Required Arguments</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/KnownFragmentNames.scala">Known Fragment Names</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/ValuesOfCorrectType.scala">Values Of Correct Type</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/UniqueDirectivesPerLocation.scala">Unique Directives Per Location</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/NoUndefinedVariables.scala">No Undefined Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/ScalarLeafs.scala">Scalar Leafs</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/UniqueArgumentNames.scala">Unique Argument Names</a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/NoFragmentCycles.scala">No Fragment Cycles</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/NoUnusedVariables.scala">No Unused Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/SingleFieldSubscriptions.scala">Single Field Subscriptions</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/NoUnusedFragments.scala">No Unused Fragments</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/UniqueVariableNames.scala">Unique Variable Names</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/UniqueInputFieldNames.scala">Unique Input Field Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/PossibleFragmentSpreads.scala">Possible Fragment Spreads</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/VariablesAreInputTypes.scala">Variables Are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/UniqueFragmentNames.scala">Unique Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/sangria-graphql/sangria/blob/main/modules/core/src/main/scala/sangria/validation/rules/VariablesInAllowedPosition.scala">Variables In Allowed Position</a></td>
		<td><a href=""></a></td>
	</tr>
</table>