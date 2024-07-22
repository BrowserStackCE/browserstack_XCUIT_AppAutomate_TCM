# browserstack_XCUIT_AppAutomate_TCM

This Github workflow is created for running XCUIT test on App Automate as well as uploading testcase, test runs on Test Management thorugh generated JUnit xml.

Below are the steps for E2E flow (App Automate to TCM)

- Upload XCUIT App on App Automate- https://www.browserstack.com/docs/app-automate/api-reference/xcuitest/apps#upload-an-app
- Upload XCUIT test suite on App Automate- https://www.browserstack.com/docs/app-automate/api-reference/xcuitest/tests#upload-a-test-suite
- Upload build using app_url and test-suite_url - https://www.browserstack.com/docs/app-automate/api-reference/xcuitest/builds#execute-a-build

- Get triggered build Status from App Automate- https://www.browserstack.com/docs/app-automate/api-reference/xcuitest/builds#get-build-status
- Fetch session ID from Build Status response and get Session Result- https://www.browserstack.com/docs/app-automate/api-reference/xcuitest/sessions#get-session-details

- Fetch instrumentation log url from session response and convert to junit XML 

- Upload jUnit XML to Test Management- https://www.browserstack.com/docs/test-management/upload-reports-cli/frameworks/xcuitest

