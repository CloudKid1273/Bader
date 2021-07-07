.cerclesi
   version:  3
   
   defaults: &defaults
     environment:
       TEST_RESULTS: /tmp/test-results
       ARTIFACT: /tmp/actifacts
       
       # we use wiki fact store in an enviroment 
       # _without_ build tool
       # correctly when build tools are missing.
jobs:
  unit-test:
    <<: *defaults 
    
