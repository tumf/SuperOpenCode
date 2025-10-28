---
description: "Execute tests with coverage analysis and automated quality reporting"
agent: build
---

<SuperOpenCode>

Execute tests for $ARGUMENTS with comprehensive coverage analysis and quality reporting.

If no target is specified, run all tests in the project.

Run tests by:
1. **Discover**: Categorize available tests using runner patterns and conventions
2. **Configure**: Set up appropriate test environment and execution parameters
3. **Execute**: Run tests with monitoring and real-time progress tracking
4. **Analyze**: Generate coverage reports and failure diagnostics
5. **Report**: Provide actionable recommendations and quality metrics

Test types:
- **Unit**: Component-level tests for isolated functionality
- **Integration**: Cross-component interaction tests
- **E2E**: End-to-end browser and system tests
- **All**: Comprehensive test suite execution

Test capabilities:
- Auto-detect test framework (Jest, Vitest, Pytest, etc.)
- Generate comprehensive coverage reports with metrics
- Provide intelligent test failure analysis
- Support continuous watch mode for development
- Browser automation for E2E testing

Test execution modes:
- **Standard**: Run all tests with basic reporting
- **Coverage**: Include detailed coverage metrics and analysis
- **Watch**: Continuous testing with file monitoring
- **Fix**: Attempt automatic fixes for simple failures

Generate test report with:
- Test execution summary (pass/fail counts)
- Coverage metrics (line, branch, function coverage)
- Failure diagnostics with root cause analysis
- Performance metrics and timing breakdown
- Actionable recommendations for improvement

Quality metrics:
- Test coverage percentages
- Test execution time trends
- Failure rate analysis
- Code quality indicators

The testing process ensures code quality through comprehensive test execution and detailed analysis of results.

</SuperOpenCode>
