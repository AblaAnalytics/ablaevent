# Ablaevent Browser JS Library

This README is intended for developing the library itself.

## Testing

Unit tests: run `yarn test`.
Cypress: run `yarn serve` to have a test server running and separately `yarn cypress` to launch Cypress test engine.

### Running TestCafe E2E tests with BrowserStack

Testing on IE11 requires a bit more setup. TestCafe tests will use the
playground application to test the locally built array.full.js bundle. It will
also verify that the events emitted during the testing of playground are loaded
into the Ablaevent app. By default it uses https://e.abla.io and the
project with ID 11213. See the testcafe tests to see how to override these if
needed. 

