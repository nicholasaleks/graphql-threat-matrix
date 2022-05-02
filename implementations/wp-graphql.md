# wp-graphql

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)
* [Notable Vulnerabilities]()

## About
Language: [php](https://www.php.net/)\
Source: [https://github.com/wp-graphql/wp-graphql](https://github.com/wp-graphql/wp-graphql)\
Documentation: [https://www.wpgraphql.com/](https://www.wpgraphql.com/)

## Security Considerations
wp-graphql provides the following features which should be taken into consideration:

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
Total Validation Count: **38**

wp-graphql is based on [graphql-php](https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-php.md) which validates the checks below as well as extra validations:

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
		<td><a href="https://github.com/wp-graphql/wp-graphql/blob/develop/src/Server/ValidationRules/RequireAuthentication.php">Require Authentication</a></td>
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

## Notable Vulnerabilities

<table>
	<tr>
		<th>CVE ID</th>
		<th>Date</th>
		<th>Score</th>
		<th>Description</th>
	</tr>
	<tr>
		<td><a href="https://www.cvedetails.com/cve/CVE-2019-9881/">CVE-2019-9881</a></td>
		<td>2019-06-10</td>
		<td>5.0</td>
		<td>The createComment mutation in the WPGraphQL 0.2.3 plugin for WordPress allows unauthenticated users to post comments on any article, even when 'allow comment' is disabled.</td>
	</tr>
	<tr>
		<td><a href="https://www.cvedetails.com/cve/CVE-2019-9880/">CVE-2019-9880</a></td>
		<td>2019-06-10</td>
		<td>6.4</td>
		<td>An issue was discovered in the WPGraphQL 0.2.3 plugin for WordPress. By querying the 'users' RootQuery, it is possible, for an unauthenticated attacker, to retrieve all WordPress users details such as email address, role, and username.</td>
	</tr>
	<tr>
		<td><a href="https://www.cvedetails.com/cve/CVE-2019-9879/">CVE-2019-9879</a></td>
		<td>2019-06-10</td>
		<td>7.5</td>
		<td>The WPGraphQL 0.2.3 plugin for WordPress allows remote attackers to register a new user with admin privileges, whenever new user registrations are allowed. This is related to the registerUser mutation.</td>
	</tr>
</table>