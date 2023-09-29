# Custom Event Handler
## Introduction / Use case.
Sample custom event handler code for testting.

## How to use.
1. Build the project using `mvn clean package` or `mvn clean package`
2. Copy the jar file `org.wso2.custom.event.handler-1.0-SNAPSHOT.jar` from the target directory to `<IS_HOME>/repository/components/dropins` folder.
3. Add the following configuration to the `<IS-HOME>/repository/conf/deployment.toml` file.
  ```
  [[event_handler]]
  name="custom.event.handler"
  subscriptions=["AUTHENTICATION_STEP_SUCCESS","AUTHENTICATION_STEP_FAILURE","AUTHENTICATION_SUCCESS","AUTHENTICATION_FAILURE","PRE_AUTHENTICATION","POST_AUTHENTICATION","PRE_SET_USER_CLAIMS","POST_SET_USER_CLAIMS","PRE_ADD_USER","POST_ADD_USER"]
  ```
