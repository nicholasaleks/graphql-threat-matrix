# jaal

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)
* [Notable Vulnerabilities](#Notable-Vulnerabilties)
* [Security Disclosure](#Security-Disclosure)

## About
Language: [go](https://go.dev/)\
Source:
- [[https://github.com/graphql-python/graphene](https://github.com/graphql-python/graphene](https://github.com/Appointy/Jaal))

Documentation: Jaal’s usage is described in its README and example code on GitHub

## Security Considerations
jaal provides the following features which should be taken into consideration:

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
  <td align="center">✅</td>   <!-- Field Suggestions -->
  <td align="center">❌</td>   <!-- Query Depth limit -->
  <td align="center">❌</td>   <!-- Query Cost -->
  <td align="center">❌</td>   <!-- APQ -->
  <td align="center">⚠️</td>   <!-- Introspection off by default -->
  <td align="center">❌</td>   <!-- Debug Mode -->
  <td align="center">❌</td>   <!-- Batch Requests -->
</tr>
</table>

## Request Validations
Total Validation Count: **24**

Jaal distributes its checks between the **query parser** (`parser.go`) and the **schema validator** (`validate.go`).  
The table lists every error it can raise, grouped under the same headings used throughout graphql-threat-matrix.

<table>
<tr>
  <th><a href="https://spec.graphql.org/October2021/#sec-Documents">Document&nbsp;Validations</a></th>
  <th><a href="https://spec.graphql.org/October2021/#sec-Validation.Operations">Operation&nbsp;Validations</a></th>
  <th><a href="https://spec.graphql.org/October2021/#sec-Validation.Fields">Field&nbsp;Validations</a></th>
  <th><a href="https://spec.graphql.org/October2021/#sec-Validation.Arguments">Argument&nbsp;Validations</a></th>
  <th><a href="https://spec.graphql.org/October2021/#sec-Validation.Fragments">Fragment&nbsp;Validations</a></th>
  <th><a href="https://spec.graphql.org/October2021/#sec-Values">Value&nbsp;Validations</a></th>
  <th><a href="https://spec.graphql.org/October2021/#sec-Validation.Variables">Variable&nbsp;Validations</a></th>
</tr>

<tr>
  <!---- Document –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">unsupported&nbsp;definition</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">must&nbsp;have&nbsp;a&nbsp;single&nbsp;query</a>
  </td>

  <!---- Operations –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">only&nbsp;supports&nbsp;query/mutation/subscription</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">only&nbsp;support&nbsp;a&nbsp;single&nbsp;query</a>
  </td>

  <!---- Fields –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">scalar&nbsp;field&nbsp;must&nbsp;have&nbsp;no&nbsp;selections</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">enum&nbsp;field&nbsp;must&nbsp;have&nbsp;no&nbsp;selections</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">object&nbsp;field&nbsp;must&nbsp;have&nbsp;selections</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">unknown&nbsp;field</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">scalar&nbsp;__typename&nbsp;must&nbsp;have&nbsp;no&nbsp;selection</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">same&nbsp;alias&nbsp;with&nbsp;different&nbsp;name</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">same&nbsp;alias&nbsp;with&nbsp;different&nbsp;args</a>
  </td>

  <!---- Arguments –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">error&nbsp;parsing&nbsp;args&nbsp;for&nbsp;field</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/validate.go">error&nbsp;parsing&nbsp;args&nbsp;for&nbsp;__typename</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">duplicate&nbsp;arg</a>
  </td>

  <!---- Fragments –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">duplicate&nbsp;fragment</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">unknown&nbsp;fragment</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">fragment&nbsp;contains&nbsp;itself</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">unused&nbsp;fragment</a>
  </td>

  <!---- Values –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">bad&nbsp;int&nbsp;arg</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">bad&nbsp;float&nbsp;arg</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">duplicate&nbsp;field&nbsp;in&nbsp;input&nbsp;object</a><br>
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">unsupported&nbsp;value&nbsp;type</a>
  </td>

  <!---- Variables –--->
  <td valign="top">
    <a href="https://github.com/appointy/jaal/blob/master/graphql/parser.go">required&nbsp;variable&nbsp;cannot&nbsp;provide&nbsp;default</a>
  </td>
</tr>
</table>
