# GraphQL API for Wordpress

### Table of Contents
* [About](#About)
* [Security Considerations](#Security-Considerations)
* [Request Validations](#Request-Validations)
* [Notable Vulnerabilities](#Notable-Vulnerabilties)
* [Security Disclosure](#Security-Disclosure)

## About
Language: [php](https://www.php.net/)\
Source: [https://github.com/leoloso/PoP](https://github.com/leoloso/PoP)\
Documentation: [https://graphql-api.com/](https://graphql-api.com/)

## Security Considerations
GraphQL API for Wordpress provides the following features which should be taken into consideration:

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
Total Validation Count: **XXX**

GraphQL API for Wordpress validates the following checks when a query is sent:

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
        <td><a href="">Executable Definitions</a></td>
        <td><a href="">Lone Anonymous Operation</a></td>
        <td><a href="">Fields on Correct Type</a></td>
        <td><a href="">Known Argument Names</a></td>
        <td><a href="">Fragments On Composite Types</a></td>
        <td><a href="">Known Type Names</a></td>
        <td><a href="">Known Directives</a></td>
        <td><a href="">No Undefined Variables</a></td>
        <td><a href="">Disable Introspection</a></td>
    </tr>
    <tr>
        <td><a href="">Lone Schema Definition</a></td>
        <td><a href="">Unique Operation Names</a></td>
        <td><a href="">Overlapping Fields Can Be Merged</a></td>
        <td><a href="">Known Argument Names On Directives</a></td>
        <td><a href="">Known Fragment Names</a></td>
        <td><a href="">Possible Type Extensions</a></td>
        <td><a href="">Unique Directive Names</a></td>
        <td><a href="">No Unused Variables</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="">Scalar Leafs</a></td>
        <td><a href="">Provided Required Arguments</a></td>
        <td><a href="">No Fragment Cycles</a></td>
        <td><a href="">Unique Enum Value Names</a></td>
        <td><a href="">Unique Directives Per Location</a></td>
        <td><a href="">Unique Variable Names</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="">Single Field Subscription</a></td>
        <td><a href="">Unique Argument Names</a></td>
        <td><a href="">No Unused Fragments</a></td>
        <td><a href="">Unique Operation Types</a></td>
        <td><a href=""></a></td>
        <td><a href="">Variables Are Input Types</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="">Unique Input Field Names</a></td>
        <td><a href="">Provided Required Arguments On Directives</a></td>
        <td><a href="">Possible Fragment Spreads</a></td>
        <td><a href="">Unique Type Names</a></td>
        <td><a href=""></a></td>
        <td><a href="">Variables In Allowed Position</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="">Unique Fragment Names</a></td>
        <td><a href="">Values Of Correct Type</a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
    </tr>
</table>

## Security Disclosure
https://graphql-api.com/contact/