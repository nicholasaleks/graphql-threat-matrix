# graphql-java

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)

## About
Language: [java](https://www.oracle.com/java/)\
Source: [https://github.com/graphql-java/graphql-java](https://github.com/graphql-java/graphql-java)\
Documentation: [https://www.graphql-java.com/](https://www.graphql-java.com/)

## Security Considerations
graphql-java provides the following features which should be taken into consideration:

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
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/ExecutableDefinitions.java">Executable Definitions</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/LoneAnonymousOperation.java">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/FieldsOnCorrectType.java">Fields On Correct Type</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/ArgumentsOfCorrectType.java">Arguments Of Correct Type</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/FragmentsOnCompositeType.java">Fragments On Composite Type</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/KnownTypeNames.java">Known Type Names</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/KnownDirectives.java">Known Directives</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/NoUndefinedVariables.java">No Undefined Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/UniqueOperationNames.java">Unique Operation Names</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/OverlappingFieldsCanBeMerged.java">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/KnownArgumentNames.java">Known Argument Names</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/ProvidedNonNullArguments.java">Provided Non Null Arguments</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/KnownFragmentNames.java">Known Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/NoUnusedVariables.java">No Unused Variables</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/ScalarLeafs.java">Scalar Leafs</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/UniqueArgumentNamesRule.java">Unique Argument Names Rule</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/NoFragmentCycles.java">No Fragment Cycles</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/NoUnusedFragments.java">No Unused Fragments</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/UniqueDirectiveNamesPerLocation.java">Unique Directive Names Per Location</a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/PossibleFragmentSpreads.java">Possible Fragment Spreads</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/UniqueVariableNamesRule.java">Unique Variable Names Rule</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/UniqueFragmentNames.java">Unique Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/VariableDefaultValuesOfCorrectType.java">Variable Default Values Of Correct Type</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/VariableTypesMatchRule.java">Variable Types Match Rule</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/VariablesAreInputTypes.java">Variables Are Input Types</a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/graphql-java/graphql-java/blob/master/src/main/java/graphql/validation/rules/VariablesTypesMatcher.java">Variables Types Matcher</a></td>
		<td><a href=""></a></td>
	</tr>
</table>