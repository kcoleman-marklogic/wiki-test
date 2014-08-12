# marklogic-samplestack

README for Version 1.0.0-ea2

Samplestack is a demo "Question and Answer" web application that shows you how to integrate MarkLogic into a three-tier application architecture (browser, application server, and database).

This release features a middle tier for the Java Enterprise Developer, implemented using Java, Spring, and Gradle.

The project includes the following major components:
* Web/browser front end based on Angular.js
* Middle appserver tier implemented in Java/Spring
* Database tier hosted on MarkLogic
* Gradle framework to drive build and configuration of the appserver and database tiers
* Unit tests

A demonstration of using MarkLogic in a three-tier application architecture.

## Getting Started
Follow this procedure to set up samplestack in your environment:

1. Install MarkLogic 8 Early Access. See http://ea.marklogic.com/download.
2. Start MarkLogic. For details, see the [MarkLogic Installation Guide](http://docs.marklogic.com/guide/installation/procedures#id_92457).
3. Clone this repository. For example, run the following command:  
        ```bash
        git clone https://github.com/marklogic/marklogic-samplestack
        ```
4. [Set up the middle and database tiers](#setting-up-the-java-middle-tier).
5. [Set up the browser tier](#setting-up-the-browser-tier).

### Setting Up the Java Middle Tier
To install required software, configure, and build the Java middle tier of
samplestack, run the following commands from the root of your cloned
repository:

```base
cd appserver/java-spring
./gradlew appserver
```

*For details, see the [README in the appserver/java-spring directory](appserver/java-spring/README.md)*

### Setting Up the Browser Tier

*For details, see the [README in the browser directory](browser/README.md)*

### Running the Application
To bring up the application in your browser, navigate to the following URL:

http://localhost:8000/XXX

## License

Copyright Â© 2014 MarkLogic

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
