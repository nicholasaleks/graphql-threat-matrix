<h1 align="center">
 <img src="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/static/graphql-threat-matrix.png?raw=true" alt="graphql-threat-matrix"/>
 <br>
</h1>

<h1 align="center">
 GraphQL Threat Matrix
</h1>

## Why graphql-threat-matrix?
[graphql-threat-matrix](https://github.com/nicholasaleks/graphql-threat-matrix) was built for bug bounty hunters, security researchers and hackers to assist with uncovering vulnerabilities across multiple GraphQL implementations.

The differences in how GraphQL implementations interpret and conform to the GraphQL specification may lead to security gaps and unique attack vectors. By analyzing and comparing the factors that drive the security risks across different implementations the GraphQL ecosystem can make safer deployment decisions as well as collectively advance the security maturity of all implementations.

<p>
<b>Legend</b><br>
✅ &nbsp;- Enabled by Default<br>
⚠️ &nbsp;- Disabled by Default<br>
❌ &nbsp;- No Support
</p>

<table>

<tr>
    <th>Implementation</th>
    <th>Validations</th>
    <th>Field Suggestions</th>
    <th>Query Depth limit</th>
    <th>Query Cost Analysis</th>
    <th>Automatic Persisted Queries</th>
    <th>Introspection</th>
    <th>Debug Mode</th>
    <th>Batch Requests</th>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/wp-graphql.md">wp-graphql</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/wp-graphql.md#Request-Validations">38</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">✅</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-php.md">graphql-php</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-php.md#Request-Validations">37</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-api-for-wp.md">graphql-api-for-wp</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-api-for-wp.md#Request-Validations">37</a></td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">✅</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/apollo.md">Apollo</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/apollo.md#Request-Validations">34</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">✅</td>
    <td align="center">✅</td>
    <td align="center">✅</td>
    <td align="center">✅</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-yoga.md">graphql-yoga</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-yoga.md#Request-Validations">34</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphene.md">graphene</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphene.md#Request-Validations">34</a></td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/ariadne.md">Ariadne</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/ariadne.md#Request-Validations">34</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/strawberry.md">Strawberry</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/strawberry.md#Request-Validations">34</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-ruby.md">graphql-ruby</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-ruby.md##Request-Validations">28</a></td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/sangria.md">Sangria</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/sangria.md#Request-Validations">27</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/tartiflette.md">Tartiflette</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/tartiflette.md#Request-Validations">26</a></td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-java.md">graphql-java</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-java.md#Request-Validations">26</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/gqlgen.md">gqlgen</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/gqlgen.md#Request-Validations">25</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/dgraph.md">Dgraph</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/dgraph.md#Request-Validations">25</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-go.md">graphql-go</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-go.md#Request-Validations">24</a></td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/juniper.md">juniper</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/juniper.md#Request-Validations">24</a></td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/diana.md">Diana.jl</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/diana.md#Request-Validations">10</a></td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/gql-dart.md">gql-dart/gql</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/gql-dart.md#Request-Validations">9</a></td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/agoo.md">Agoo</a></td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/agoo.md#Request-Validations">1</a></td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
</tr>
<tr>
 <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/lighthouse.md">Lighthouse</a></td>
 <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/lighthouse.md#Request-Validations">1</a></td>
		<td align="center">✅</td>
		<td align="center">⚠️</td>
		<td align="center">⚠️</td>
		<td align="center">⚠️</td>
		<td align="center">✅</td>
		<td align="center">⚠️</td>
		<td align="center">✅</td>
</tr>

</table>

## For Penetration Testers
Use [graphw00f](https://github.com/dolevf/graphw00f) to fingerprint a target GraphQL API and determine the backend implementation.

## Want to provide a submission (or correction)?
Interested in contributing? Found a discrepancy? Please create a GitHub issue or PR with your details.

## Contributors & Maintainers
- [Nick Aleks](https://github.com/nicholasaleks)
- [Dolev Farhi](https://github.com/dolevf)
