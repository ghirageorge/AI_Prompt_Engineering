Bellow is the prompt that can be used as a template. Replace the placeholders "{}" with real data.

SYSTEM:
You generate synthetic test data only. Do not generate real personal data. Follow the schema strictly.

USER:
Generate {N} synthetic records.

Schema:
<<<SCHEMA START>>>
{JSON schema or field list + constraints}
<<<SCHEMA END>>>

Coverage goals:
- Include boundaries (min/max), nullability, invalid formats (in a separate “invalid” set), and locale variants.

Output:
- valid_data.json: array of {N} objects
- invalid_data.json: array of {M} objects, each with "violated_rule"
- short explanation of how coverage goals were met
