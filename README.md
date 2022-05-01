<h1 align="center">
 <img src="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/static/graphql-threat-matrix.png?raw=true" alt="graphql-threat-matrix"/>
 <br>
</h1>

<h1 align="center">
 GraphQL Threat Matrix
</h1>


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
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-php.md">graphql-php</td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-php.md#Validations">37</a></td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">⚠️</td>
    <td align="center">⚠️</td>
</tr>

<tr>
    <td>graphql-js</td>
    <td align="center">34</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
</tr>

<tr>
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-ruby.md">graphql-ruby</td>
    <td align="center"><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/graphql-ruby.md#Validations">28</a></td>
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
    <td><a href="https://github.com/nicholasaleks/graphql-threat-matrix/blob/master/implementations/gqlgen.md">gqlgen</td>
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
    <td>graphql-core</td>
    <td align="center">24</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
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
    <td>graphql-rust</td>
    <td align="center">24</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
</tr>

<tr>
    <td>Diana.jl</td>
    <td align="center">10</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
    <td align="center">✅</td>
    <td align="center">❌</td>
    <td align="center">❌</td>
</tr>

</table>