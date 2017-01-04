example usage:

1. launch application with

    mvn clean jetty:run

2. test / extract

    - DOLCE ontology
        
        http://localhost:8080/lode/extract?url=http://www.loa.istc.cnr.it/ontologies/DOLCE-Lite.owl
    
    - photography ontology
    
        http://localhost:8080/lode/extract?url=http://130.88.198.11/co-ode-files/ontologies/photography.owl

    - serve local owl file
        `riot --output=rdfxml your.ttl > your.owl`
        `curl -X POST --data-binary @your.owl --header "Content-Type:application/xml" http://localhost:8080/lode/extract\ > your.html`