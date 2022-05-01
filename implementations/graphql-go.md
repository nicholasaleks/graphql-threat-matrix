# graphql-go

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request-Validations](#Request-Validations)

## About
Language: [go](https://go.dev/)\
Source: [https://github.com/graphql-go/graphql](https://github.com/graphql-go/graphql)\
Documentation: [https://pkg.go.dev/github.com/graphql-go/graphql](https://pkg.go.dev/github.com/graphql-go/graphql)

## Security Considerations
GraphQL Go provides the following features which should be taken into consideration:

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
		<td align="center">⚠️<br>Disabled by Default</td>
		<td align="center">❌<br>No Support</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **24**

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
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go"></a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Lone Anonymous Operation</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Fields on Correct Type</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Arguments of Correct Type</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Fragments on Composite Types</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Default Value of Correct Type</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Known Directives</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">No Undefined Variables</a></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Unique Operation Names</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Overlapping Fields Can Be Merged</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Known Argument Names</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Known Fragment Names</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Known Type Names</a></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">No Unused Variables</a></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Scalar Leafs</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Provided Non Null Arguments</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">No Unused Fragments</a></td>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Unique Variable Names</a></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Unique Input Field Names</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Unique Argument Name</a></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Possible Fragment Spreads</a></td>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Variables Are Input Types</a></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td></td>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Unique Fragment Names</a></td>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">Variables In Allowed position</a></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td></td>
		<td></td>
		<td></td>
		<td><a href="https://github.com/graphql-go/graphql/blob/master/rules.go">No Fragment Cycles</a></td>
		<td></td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
</table>