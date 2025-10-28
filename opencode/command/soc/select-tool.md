---
description: "Analyze operation and recommend optimal tool selection strategy"
subtask: true
---

<SuperOpenCode>

Analyze the operation and recommend the optimal tool or approach for execution.

Perform tool selection by:
1. **Parse**: Analyze operation type, scope, and complexity indicators
2. **Score**: Apply complexity scoring across operation factors
3. **Match**: Compare requirements against available tool capabilities
4. **Select**: Choose optimal tool based on scoring and requirements
5. **Validate**: Verify selection accuracy and provide confidence metrics

Tool selection factors:
- **Operation Type**: Symbol operations, pattern edits, memory operations
- **Scope**: File count, lines of code, impact radius
- **Complexity**: Language features, framework patterns, dependency depth
- **Performance**: Speed vs accuracy trade-offs

Decision criteria:
- **Semantic Operations**: Complex refactoring, symbol navigation, LSP features
- **Pattern Operations**: Bulk edits, string replacements, format changes
- **Memory Operations**: Context persistence, session management
- **Speed Critical**: Simple operations requiring fast execution

Complexity scoring:
- File count and scope analysis
- Operation type classification
- Language and framework requirements
- Performance vs accuracy needs

Generate recommendation with:
- Selected tool and rationale
- Complexity score breakdown
- Trade-off analysis
- Confidence metrics
- Alternative approaches

The tool selection process ensures optimal performance and accuracy by matching operations with appropriate tools.

</SuperOpenCode>
