---
sidebar_position: 2
---

# Configuration

Use config.yml file to specify your fault simulation and schema coverage strategy

This is an example of a configuration with different types of faults, 
```text title="config.yml"
// highlight-start
faults:
  null_field:
    enabled: true
  missing_field:
    enabled: true
  invalid_data_type:
    enabled: false
  invalid_value:
    enabled: true
  http_method_change:
    enabled: false
  status_code_change:
    enabled: false
  delay_injection:
    enabled: false
    delay_ms: 500

base_uri: "api.yourapp.io"

endpoints:
  exclude:
    - '*/login*'
tests:
  exclude:
    - '*login*'

report:
  format: json
  output_path: "./reports/simulator-report.json"

schema_coverage:
    open_api_spec: "local-path-or-url.yml"
    report_ouput_path: "./reports/schema-coverage.json"
// highlight-end


