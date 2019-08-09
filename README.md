# mulesoft-pocs
POC work with Mule Soft Concepts uisng Mule 4

# job-details-sapi:  showcasing Mule 4 Rest API Definition and Implementation.
     1. RAML datatypes,RAML Library,RAML Traits,resource Definitions.
     2. Oraganizing mule resources(api,api-console,api-impl,implementation,common-error,global-config)
     3. Used Secure Properties, JSON Logger
     4. API Discovery
     5. Munit test cases.
# Shared-logger: Mule 4 implementation of sahred logging framework to be used by all mule Service in network
     1. dependant flows has to initialize sharedLogData arraylist variable
     2. to log transport and status from dependant flows, a json data variable(traceVariable) should be initalized
          ex: traceVariable ={"transport":"MQ-PUT","status:END"}
              traceVariable ={"transport":"DB-INSERT"}
     3. dependant flows need to reference "shared-logger"  flower to capture log entry.
     4. KB artcle using shared flows.
      https://support.mulesoft.com/s/article/How-to-add-a-call-to-an-external-flow-in-Mule-4
      

     
