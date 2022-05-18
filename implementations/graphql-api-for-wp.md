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
        <td align="center">⚠️<br>Disabled by Default</td>
        <td align="center">❌<br>No Support</td>
        <td align="center">❌<br>No Support</td>
        <td align="center">✅<br>Enabled by Default</td>
        <td align="center">✅<br>Enabled by Default</td>
        <td align="center">⚠️<br>Disabled by Default</td>
        <td align="center">✅<br>Enabled by Default</td>
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
        <td><a href="https://github.com/leoloso/PoP/blob/21f5820c459800946ad69b530412eded836e4f1e/layers/Engine/packages/graphql-parser/src/Spec/Parser/Parser.php">Executable Definitions</a> <= This is implicit, because the server is code-first: it doesn't handle SDL, hence non-executable definitions are directly not supported, and the parser will already throw an error</td>
        <td><a href="https://github.com/leoloso/PoP/blob/45791105a1b850ee1b07426700c476440d43f4c0/layers/Engine/packages/graphql-parser/src/Spec/Execution/ExecutableDocument.php#L87">Lone Anonymous Operation</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/dbba064860c3df23d5731f909902243b74cb1aa1/layers/Engine/packages/component-model/src/TypeResolvers/ObjectType/AbstractObjectTypeResolver.php#L172">Fields on Correct Type</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/dbba064860c3df23d5731f909902243b74cb1aa1/layers/Engine/packages/component-model/src/Schema/FieldQueryInterpreter.php#L465">Known Argument Names</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/9c05560107a1d7163f494aee742fc2cea5149a39/layers/Engine/packages/component-model/src/ExtendedSpec/Execution/ExecutableDocument.php#L111">Fragments On Composite Types</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/dbba064860c3df23d5731f909902243b74cb1aa1/layers/Engine/packages/component-model/src/TypeResolvers/UnionType/AbstractUnionTypeResolver.php#L414">Known Type Names</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/dbba064860c3df23d5731f909902243b74cb1aa1/layers/Engine/packages/component-model/src/TypeResolvers/AbstractRelationalTypeResolver.php#L248">Known Directives</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L383">No Undefined Variables</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/a90db0edd3fb7dc85edc434adc3e48fb41c75356/layers/GraphQLAPIForWP/plugins/graphql-api-for-wp/docs/en/release-notes/0.9.md#exposed-the-__schema-introspection-field-in-the-acls">Disable Introspection</a></td>
    </tr>
    <tr>
        <td><a href="">Lone Schema Definition</a> <= Same as above, no SDL is supported, so no "schema" can be passed in the query</td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L128">Unique Operation Names</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/21f5820c459800946ad69b530412eded836e4f1e/layers/Engine/packages/graphql-parser/src/Spec/Parser/Parser.php#L660">Unique Input Field Names</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/dbba064860c3df23d5731f909902243b74cb1aa1/layers/Engine/packages/component-model/src/Schema/FieldQueryInterpreter.php#L465">Known Argument Names On Directives</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L173">Known Fragment Names</a></td>
        <td><a href="">Possible Type Extensions</a> <= Same as above, no SDL is supported, so no "type extensions" supported</td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L566">No Unused Variables</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/215b00a97789b3b543adc2f3380d1ca8f705a2f6/layers/Engine/packages/component-model/src/Resolvers/FieldOrDirectiveResolverTrait.php#L26">Provided Required Arguments</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L276">No Fragment Cycles</a></td>
        <td><a href="">Unique Enum Value Names</a> <= Same as above, as the definition is via code and not SDL, this issue is impossible to happen</td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L357">Unique Variable Names</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L667">Unique Argument Names</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L312">No Unused Fragments</a></td>
        <td><a href="">Unique Type Names</a> <= Same as above, as the definition is via code and not SDL, this issue is impossible to happen</td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/45791105a1b850ee1b07426700c476440d43f4c0/layers/Engine/packages/graphql-parser/src/Spec/Execution/ExecutableDocument.php#L129">Variables In Allowed Position</a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/215b00a97789b3b543adc2f3380d1ca8f705a2f6/layers/Engine/packages/component-model/src/Resolvers/FieldOrDirectiveResolverTrait.php#L26">Provided Required Arguments On Directives</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/9c05560107a1d7163f494aee742fc2cea5149a39/layers/Engine/packages/component-model/src/ExtendedSpec/Execution/ExecutableDocument.php#L93">Possible Fragment Spreads</a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/dbba064860c3df23d5731f909902243b74cb1aa1/layers/Engine/packages/component-model/src/Schema/FieldQueryInterpreter.php#L1021">Values Of Correct Type</a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
    </tr>
    <tr>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href="https://github.com/leoloso/PoP/blob/56beb22e72795e7a4ba61f33a1b75ee91e551407/layers/Engine/packages/graphql-parser/src/Spec/Parser/Ast/Document.php#L261">Unique Fragment Names</a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
        <td><a href=""></a></td>
    </tr>
</table>

## Security Disclosure
https://graphql-api.com/contact/