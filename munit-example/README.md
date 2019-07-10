# MUnit Example

## Things to Note
- The tests use the Dataweave dw::utils::Diff library to assert that the JSON structure returned at the end of flow matches the output format defined in the RAML, without caring about order of the key-value pairs on the objects. 
- Mocks can be used to mock calls to external resources or other flows.
- _Verify Call_ can be used to verify that a particular processor was executed in the flow. This is useful on flows that have Choice Routers to assert that a particular route was executed.

## Running Tests in Studio
- Navigate to src/test/munit
- Right click on canvas and select _Run MUnit suite_

## Running Tests from Command Line
- Maven must be installed and the executable must be in the path
- ~/.m2/settings.xml must be configured to pull in Mule Enterprise dependencies
- Navigate to the root of the project
- Run `mvn clean test`
