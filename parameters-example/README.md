# Using Parameters in CloudHub

## Things to Note
- Application parameters are stored in config.yaml in src/main/resources
- Values intended to be encrypted in CloudHub should be listed in _mule-artifact.json_ in the root of the project

```JSON
{
  "minMuleVersion": "4.2.0",
  "secureProperties": ["properties.secret"]
}
```

- Values can be updated in Runtime Manager.
- Values listed in the secureProperties list will be encrypted and hidden in Runtime Manager
