# Best of Java Libraries
List of libraries I recommend to use for Java projects &amp; libraries I'd like to use.

At the moment this list is not complete, but I'll try to add most of libraries I've ever worked with.

## Application Glue (IoC, DI, etc.)
#### Battle tested
- [Spring Framework](https://projects.spring.io/spring-framework/) - Well known DI & much-much more.
- [OSGi - Equinox](http://www.eclipse.org/equinox/) - Very specific modular framework, overkill for most applications.

#### Waiting for reviews
- [Google Guice](https://github.com/google/guice) - Minimalistic implementation of [JSR-330](https://www.jcp.org/en/jsr/detail?id=330) (standardizes annotations like ```@Inject``` and the ```Provider```).

## Micro-Frameworks for Web Applications
#### Waiting for reviews
- [Rapidoid](http://www.rapidoid.org) - Extremely Fast, Simple and Powerful Java Web Framework!

## Microservices & Distributed Computation
#### Waiting for reviews
- [Akka](http://akka.io) - A toolkit and runtime for building highly concurrent, distributed, and resilient message-driven applications.
- [Netflix - Hystrix](https://github.com/Netflix/Hystrix) - A latency and fault tolerance library.
- [Netflix - Eureka](https://github.com/Netflix/eureka) - Service registry.
- [Netflix - Ribbon](https://github.com/Netflix/ribbon) - A Inter Process Communication (RPC) library with built in software load balancers.
- [Netflix - EVCache](https://github.com/Netflix/EVCache) - A distributed in-memory data store for the cloud. 
- [Netflix - Zuul](https://github.com/Netflix/zuul) - A gateway service that provides dynamic routing, monitoring, resiliency, security, and more.
- [Zipkin](http://zipkin.io/) - A distributed tracing system. It helps gather timing data needed to troubleshoot latency problems.

## Build tools
#### Battle tested
- [Maven](https://maven.apache.org/download.cgi) - This is Maven: solid but not flexible.
- [Gradle](https://gradle.org/) - Cool, but require a lot of discipline in order not to generate mess in build scripts.

#### Waiting for reviews
- [Bazel](https://bazel.build/) - Language agnostic tool that automates software builds and tests.

## Computation Frameworks
#### Battle tested
- [Apache Spark](http://spark.apache.org) - Great distributed computing platform.

#### Waiting for reviews
- [Apache Storm](http://storm-project.net/) - A free and open source distributed realtime computation system.
- [Presto](https://prestodb.io/) - Distributed SQL Query Engine for Big Data.
- [Twitter Finagle](https://twitter.github.io/finagle/) - An extensible RPC system for the JVM, used to construct high-concurrency servers.

## General Purpose Libraries (Collections, Networking, Monitoring, etc.)
#### Battle tested
- [RxJava](https://github.com/ReactiveX/RxJava) - A library for composing asynchronous and event-based programs using observable sequences.
- [Guava](https://github.com/google/guava) - Google provided utiities for things you missing in Java SDK.
- [Dropwizard Metrics](https://github.com/dropwizard/metrics) - Application-level metrics.
- [FasterXML Jackson](https://github.com/FasterXML/jackson) - Great XML/JSON/etc. <-> POJO converter.
- [Project Lombock](https://projectlombok.org/) - Boilerplate genertion.
- [Ehcache](http://www.ehcache.org) - In-memory cache for Java.
- [JNA](https://github.com/java-native-access/jna) - Simple but powerfull integration with native code.

#### Waiting for reviews
- [okhhtp](https://github.com/square/okhttp) - An HTTP+HTTP/2 client for Android and Java applications.
- [leakcanary](https://github.com/square/leakcanary) - A memory leak detection library for Android and Java.
- [Unirest](http://unirest.io/) - Lightweight HTTP Request Client Libraries.
- [Retrofit](http://square.github.io/retrofit/) - A type-safe HTTP client for Android and Java.
- [JDeferred](http://jdeferred.org/) - is a Java Deferred/Promise library similar to JQuery's Deferred Object.
- [Project Reactor](https://projectreactor.io/) - fourth-generation Reactive library for building non-blocking applications on the JVM based on the [Reactive Streams Specification](https://github.com/reactive-streams/reactive-streams-jvm). Spring friendly.
- [Javaslang](http://www.javaslang.io/) - Functional programming in Java.
- [JavaPoet](https://github.com/square/javapoet) - A Java API for generating .java source files.
- [Netflix Hollow]() - comprehensive toolset for harnessing small to moderately sized in-memory datasets.
- [JavaSpark](https://github.com/perwendel/spark) - A tiny web framework for Java 8.
- [okio](https://github.com/square/okio) - A modern I/O API for Java.
- [JCTools](https://github.com/JCTools/JCTools) - Concurrent data structures currently missing from the JDK.
- [MapStruct](http://mapstruct.org) - An annotation processor for DTO mapping (compile-time).

## DB & Integration Tools
#### Battle tested
- [EclipseLink](http://www.eclipse.org/eclipselink/) - Ok JPA implementation (and much more), need to be carefull with big projects.

#### Waiting for reviews
- [Hibernate](http://hibernate.org/) - Idiomatic persistence for Java and relational databases. 
- [HikariCP](https://github.com/brettwooldridge/HikariCP) - high-performance JDBC connection pool.
- [Liquibase](http://www.liquibase.org/) - DB migration library.
- [QueryDSL](http://www.querydsl.com/) - DB integration helper tool.
- [Slik](http://slick.lightbend.com/) - Scala library for functional relational mapping.
- [Titan DB](http://titan.thinkaurelius.com/) - A scalable graph database optimized for storing and querying graphs containing hundreds of billions of vertices and edges distributed across a multi-machine cluster.

## Application Integration & Messaging (EIP)
#### Battle tested
- [Apache ActiveMQ](http://activemq.apache.org/) - Message broker, JMS implementation. Old & has a lot of design issues, in most cases it is overkill.
- [Apache Camel](http://camel.apache.org/) - Powerfull implementation of EIP, but in modern applications it is rearly usefull.

#### Waiting for reviews
- [Apache Kafka](https://kafka.apache.org/) - Used for building real-time data pipelines and streaming apps.

## Application Testing (Unit, Integration)
#### Battle tested
- [JUnit](http://junit.org/junit5) - Just JUnit.
- [TestNG](http://testng.org/doc/index.html) - Just TestNG.
- [Mockito](http://site.mockito.org) - Mocking library. 
- [JMH](http://openjdk.java.net/projects/code-tools/jmh/) - Best option for micro-benchmarks in Java!
- [RestAssured](https://github.com/rest-assured/rest-assured) - DSL for testing REST API.
- [H2](http://www.h2database.com/html/tutorial.html) - Great for faking more serious SQL databases.
- [Fongo](https://github.com/fakemongo/fongo) - Fast dummy Mongo API compatible inmemory replacement, gread for tests.
- [Embedded Mongo](https://github.com/flapdoodle-oss/de.flapdoodle.embed.mongo) - Great way to bring MongoDB into test, but could be slow & require native (platform dependent libraries).
- [JimFS](https://github.com/google/jimfs) - Goole library for testing file system related workflows.

#### Waiting for reviews
- [JUnit Theories](https://github.com/junit-team/junit4/wiki/theories) - Yet unexplored JUnit feature for property based testing.
- [WireMock](http://wiremock.org) - Mock HTTP services in tests.
- [PiTest](http://pitest.org) - Mutation testing.
- [junit-quickcheck](https://github.com/pholser/junit-quickcheck) - Property based testing for JUnit.
- [Spock](http://spockframework.org/) - It is Groovy library, but in Java projects Groovy often used for testing.
- [Awaitability](https://github.com/awaitility/awaitility) - Helper library for async software testing.
- [ScalaCheck](https://www.scalacheck.org/) - Property based testing.

## Java & GPU Computation
#### Waiting for reviews
- [AMD Aparapi](http://aparapi.github.io/) - AMD implementation of Java to OpenCL interface.
- [aparapi](https://github.com/Syncleus/aparapi) - a framework for executing native Java code on the GPU.
