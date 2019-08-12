# mulesoft-pocs
POC work with Mule Soft Concepts uisng Mule 4

# job-details-sapi:  showcasing Mule 4 Rest API Definition and Implementation.
     1. RAML datatypes,RAML Library,RAML Traits,resource Definitions.
     2. Oraganizing mule resources(api,api-console,api-impl,implementation,common-error,global-config)
     3. Used Secure Properties, JSON Logger
     4. API Discovery
     5. Munit test cases.
# Shared-logger: Mule 4 implementation of a shared logging framework for all mule Services in network
     1. dependant flows has to initialize sharedLogData arraylist variable
     2. to log transport and status from dependant flows, a json data variable(traceVariable) should be initalized
          ex: traceVariable ={"transport":"MQ-PUT","status:END"}
              traceVariable ={"transport":"DB-INSERT"}
     3. dependant flows need to reference "shared-logger"  flower to capture log entry.
     4. KB artcle using shared flows.
      https://support.mulesoft.com/s/article/How-to-add-a-call-to-an-external-flow-in-Mule-4
# poc-exception-handling: Mule 4 implementation of a common exception handling framework for all mule Services in network
     1. dependant flows has to reference the global onError-Propagate and OnError-Continue flows as needed.
     2. common errors can be defined in two categories in configuration files.
           a.) Propagatation Errors. (Includes Custom API mapping Errors)
           b). Continue Errors. (Includes Custom API mapping Errors)
      3. API specifc errors can also be defined in configuration files so framework resolves the errorCode and errorDescription 
         dynamically.
     4. KB artcle using shared flows.
      https://support.mulesoft.com/s/article/How-to-add-a-call-to-an-external-flow-in-Mule-4      

     
