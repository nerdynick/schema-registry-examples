# schema-registry-examples
Collection of examples and ideas for managing Schema and Subjects within the Confluent Schema Registry

## schema-registry-examples-register

In this example we will show how to:
1. Manage your schemas centrally.
2. Automate registration of those schemas against Subject.
3. Package & distribute a Jar dependency containing POJO builds of your schemas.  

This examples makes use of 2 Maven Plugins:
1. [avro-maven-plugin](https://avro.apache.org/docs/current/gettingstartedjava.html) - 
    Apache Avro Maven Plugin to compile Avro (.avsc) files into POJOs. For use within your codebase.
2. [kafka-schema-registry-maven-plugin](https://docs.confluent.io/current/schema-registry/develop/maven-plugin.html#sr-maven-plugin) - 
    Confluent Schema Registry Plugin used to [register](https://docs.confluent.io/current/schema-registry/develop/maven-plugin.html#schema-registry-register) and update your schema definitions against a Schema Registry instance. 

## schema-registry-examples-download

In this example we will show how to:
1. Download schema definitions from the Confluent Schema Registry.
2. Compile those schema definitions into POJOs for use within our codebase.

This examples makes use of 2 Maven Plugins:
1. avro-maven-plugin - 
    Apache Avro Maven Plugin to compile Avro (.avsc) files into POJOs. For use within your codebase.
2. kafka-schema-registry-maven-plugin - 
    Confluent Schema Registry Plugin used to [download](https://docs.confluent.io/current/schema-registry/develop/maven-plugin.html#schema-registry-download) your schema definitions from a Schema Registry instance.  