# Diana.jl

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)
* [Security Disclosure](#Security-Disclosure)

## About
Language: [julia](https://julialang.org/)\
Source: [https://github.com/neomatrixcode/Diana.jl](https://github.com/neomatrixcode/Diana.jl)\
Documentation: [https://diana.nicepage.io/](https://diana.nicepage.io/)

## Security Considerations
diana.jl provides the following features which should be taken into consideration:

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
		<td align="center">⚠️<br>Disabled by Default</td>
	</tr>
</table>

## Request Validations
Total Validation Count: **10**

diana.jl validates the following checks when a query is sent:

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
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Not Extension On Operation</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Fragment Subscription</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Not Type on Operation</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Fragment Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Not Schema on Operation</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Fragment Unknown Not Used</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Operation Names</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Fragment Cycles</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Operation Anonymous</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
	<tr>
		<td><a href=""></a></td>
		<td><a href="https://github.com/neomatrixcode/Diana.jl/blob/master/src/rules/consultas.jl">Subscription Fields</a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
		<td><a href=""></a></td>
	</tr>
</table>

## Security Disclosure
https://github.com/neomatrixcode/Diana.jl/issues