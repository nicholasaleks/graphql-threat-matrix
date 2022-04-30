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
Total Validation Count: **26**

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
		<td><a href="">Possible Types</a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Selection Set</a></td>
		<td><a href="">Arguments Conflict</a></td>
		<td><a href="">Mark Used Fragments</a></td>
		<td><a href="">Validate Value</a></td>
		<td><a href="">Validate Directives</a></td>
		<td><a href="">Can Be Input</a></td>
		<td><a href="">Validate Max Depth</a></td>
	</tr>
	<tr>
		<td><a href="">Validate Name</a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Selections</a></td>
		<td><a href="">Validate Argument Types</a></td>
		<td><a href="">Detect Fragment Cycle</a></td>
		<td><a href="">Validate Value Type</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Literal</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Overlap</a></td>
		<td><a href="">Validate Argument Literals</a></td>
		<td><a href="">Detect Fragment Cycle Selection Set</a></td>
		<td><a href="">Types Compatible</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Basic Lit</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Field Overlap</a></td>
		<td><a href="">Can Be Fragment</a></td>
		<td><a href=""></a></td>
		<td><a href="">Types Can Be Used As</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Validate Builtin Scalar</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Has Subfields</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Is Null</a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="">Is Leaf</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>