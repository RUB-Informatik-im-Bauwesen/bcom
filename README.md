Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# Building Concrete Monitoring Ontology (BCOM)

## Metadata
* **IRI**
  * `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring`
* **Creators(s)**
  * Liu Liu, Ruhr-University Bochum
  * Philipp Hagedorn, Ruhr-University Bochum
* **Created**
  * 2021-01-20
* **Version Information**
  * 0.2
* **License**
  * [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
* **Source**
  * [https://github.com/RUB-Informatik-im-Bauwesen/bcom](https://github.com/RUB-Informatik-im-Bauwesen/bcom)
* **Ontology RDF**
  * RDF ([BuildingConcreteMonitoring.ttl](turtle))
### Description
<p>The Building Concrete Monitoring Ontology (BCOM) is defined for capturing information of concrete work, concrete curing and testing of concrete properties.</p>

## Table of Contents
1. [Classes](#classes)
1. [Object Properties](#objectproperties)
1. [Datatype Properties](#datatypeproperties)
1. [Namespaces](#namespaces)
1. [Legend](#legend)


## Overview
![Overview of Ontology](https://icdd.vm.rub.de/ontology/bcom/BuildingConcreteMonitoring.png "Overview of Ontology")  
**Figure 1:** Ontology overview
## Classes
[Concrete curing](#Concretecuring),
[Concrete delivery](#Concretedelivery),
[Concrete placement](#Concreteplacement),
[Conformity testing of compressive strength](#Conformitytestingofcompressivestrength),
[Fresh concrete property testing](#Freshconcretepropertytesting),
[Storage of a test sample](#Storageofatestsample),
[Test](#Test),
[Test sample](#Testsample),
### Concrete curing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring`
Description | <p>This class provides the necessary information of concrete curing after concreting</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BeginDate](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BeginDate) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MinAirTemperature](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MinAirTemperature) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EndDate](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EndDate) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MaxAirTemperature](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MaxAirTemperature) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MethodOfAftertreatment](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MethodOfAftertreatment) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasConcretePlacement) (op)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasCuring) (op)<br />
### Concrete delivery
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery`
Description | <p>This class provides information about the delivery of concrete</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliveryNote](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliveryNote) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EndTimeOfPlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EndTimeOfPlacement) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BeginTimeOfPlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BeginTimeOfPlacement) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasSupplier](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasSupplier) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliversConcreteFor](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliversConcreteFor) (op)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasDelivery) (op)<br />
### Concrete placement
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement`
Description | <p>This class provides the necessary information of current concreting of the construction</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#QuantityOfConcrete](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#QuantityOfConcrete) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ClassOfMonitoring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ClassOfMonitoring) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasCuring) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DateOfStripping](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DateOfStripping) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DateOfConcreting](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DateOfConcreting) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteTemperature](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteTemperature) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasDelivery) (op)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SuppliesConcreteTo](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SuppliesConcreteTo) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliversConcreteFor](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliversConcreteFor) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasConcretePlacement) (op)<br />
### Conformity testing of compressive strength
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength`
Description | <p>This class provides the necessary information to perform and evaluate the conformity testing of concrete compressive strength.</p>
Super-classes |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestedBreakingLoad](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestedBreakingLoad) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EvaluationOfTest](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EvaluationOfTest) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#InterimCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#InterimCompressiveStrength) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#NormativeReference](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#NormativeReference) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FinalCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FinalCompressiveStrength) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConversionFactor](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConversionFactor) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestCharacteristic](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestCharacteristic) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestedDensity](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestedDensity) (dp)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTest](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTest) (op)<br />
### Fresh concrete property testing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties`
Description | <p>This class represents a group of fresh concrete property.  A fresh concrete property set object will usually contain density, voids ratio, consistency.</p>
Super-classes |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#VoidsRatio](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#VoidsRatio) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#RateOfFlowTableTest](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#RateOfFlowTableTest) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MaturityOfConcrete](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MaturityOfConcrete) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BulkDensity](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BulkDensity) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteTemperature](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteTemperature) (dp)<br />
### Storage of a test sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage`
Description | <p>This class represents the storage conditions of a test sample</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Humidity](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Humidity) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Temperature](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Temperature) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Duration](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Duration) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Condition](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Condition) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#StoresSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#StoresSample) (op)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasStorage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasStorage) (op)<br />
### Test
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test`
Description | <p>Represents the super-class for different types of tests for placed concrete</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties) (c)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTest](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTest) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestTime](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestTime) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestPerson](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestPerson) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestOrganisation](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestOrganisation) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestDate](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestDate) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSample) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestReport](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestReport) (dp)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSubjects](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSubjects) (op)<br />
### Test sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample`
Description | <p>This class provides the information of test sample for conformity test of concrete compressive strength</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ObjectTemperature](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ObjectTemperature) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Weigth](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Weigth) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Height](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Height) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SamplingDate](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SamplingDate) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SampleID](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SampleID) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasStorage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasStorage) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#WidthOrDia](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#WidthOrDia) (dp)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Length](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Length) (dp)<br />
In range of |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSample) (op)<br />[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#StoresSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#StoresSample) (op)<br />

## Object Properties
[Delivers concrete for](#Deliversconcretefor),
[Curing has Concrete Work](#CuringhasConcreteWork),
[has Curing](#hasCuring),
[has Concrete Supplier](#hasConcreteSupplier),
[HasStorage](#HasStorage),
[has Concrete Supplier](#HasSupplier),
[has Test Of Compressive Strength](#hasTestOfCompressiveStrength),
[has Perform Test Organisation](#hasPerformTestOrganisation),
[has Perform Test Person](#hasPerformTestPerson),
[has Test Sample](#hasTestSample),
[has Test Subjects](#hasTestSubjects),
[StoresSample](#StoresSample),
[supplies Concrete to](#suppliesConcreteto),
[](Deliversconcretefor)
### Delivers concrete for
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliversConcreteFor`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
[](CuringhasConcreteWork)
### Curing has Concrete Work
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasConcretePlacement`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
[](hasCuring)
### has Curing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasCuring`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
[](hasConcreteSupplier)
### has Concrete Supplier
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasDelivery`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery) (c)<br />
[](HasStorage)
### HasStorage
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasStorage`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage) (c)<br />
[](HasSupplier)
### has Concrete Supplier
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasSupplier`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery) (c)<br />
Range(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
[](hasTestOfCompressiveStrength)
### has Test Of Compressive Strength
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTest`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
[](hasPerformTestOrganisation)
### has Perform Test Organisation
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestOrganisation`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
[](hasPerformTestPerson)
### has Perform Test Person
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestPerson`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[vcard:Individual](http://www.w3.org/2006/vcard/ns#Individual) (c)<br />
[](hasTestSample)
### has Test Sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSample`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
[](hasTestSubjects)
### has Test Subjects
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#HasTestSubjects`
Domain(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
[](StoresSample)
### StoresSample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#StoresSample`
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
[](suppliesConcreteto)
### supplies Concrete to
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SuppliesConcreteTo`
Domain(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
Range(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />

## Datatype Properties
[Air temperature](#Airtemperature),
[Begin date of concrete curing](#Begindateofconcretecuring),
[Begin time of paving](#Begintimeofpaving),
[Bulk density](#Bulkdensity),
[Class Of concrete monitoring](#ClassOfconcretemonitoring),
[Fresh concrete temperature](#Freshconcretetemperature),
[Storage condition](#Storagecondition),
[Conversion factor](#Conversionfactor),
[Date of concreting](#Dateofconcreting),
[Date of stripping](#Dateofstripping),
[Delivery note](#Deliverynote),
[Storage duration](#Storageduration),
[End date of concrete curing](#Enddateofconcretecuring),
[End time of paving](#Endtimeofpaving),
[Evaluation of the mean value](#Evaluationofthemeanvalue),
[Result of compressive strength](#Resultofcompressivestrength),
[Fresh concrete temperature before concreting](#Freshconcretetemperaturebeforeconcreting),
[Height of sample](#Heightofsample),
[Storage humidity](#Storagehumidity),
[Intermediate result of compressive strength](#Intermediateresultofcompressivestrength),
[Length of sample](#Lengthofsample),
[Maturity of concrete](#Maturityofconcrete),
[Max temperature](#Maxtemperature),
[Method of concrete curing](#Methodofconcretecuring),
[Min temperature](#Mintemperature),
[Test standard](#Teststandard),
[Temperature of sample](#Temperatureofsample),
[Quantity of concrete](#Quantityofconcrete),
[Rate of flow table test](#Rateofflowtabletest),
[Sample ID](#SampleID),
[Date of sampling](#Dateofsampling),
[Storage temperature](#Storagetemperature),
[Tested property](#Testedproperty),
[Date of testing](#Dateoftesting),
[Test report](#Testreport),
[Time of testing](#Timeoftesting),
[Type of test](#Typeoftest),
[Value of breaking load](#Valueofbreakingload),
[Density of sample](#Densityofsample),
[Voids ratio](#Voidsratio),
[Weigth of sample](#Weigthofsample),
[Width or diameter of sample](#Widthordiameterofsample),
[](Airtemperature)
### Air temperature
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#AirTemperature`
Description | Air temperature during concreting or test on fresh concrete in Celsius
Domain(s) |([http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c) or [http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c))<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Begindateofconcretecuring)
### Begin date of concrete curing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BeginDate`
Description | Begin date of concrete curing with format year-month-day in yyyy-mm-dd
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Begintimeofpaving)
### Begin time of paving
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BeginTimeOfPlacement`
Description | Begin time of paving with format hour-minute-second in hh-mm-ss
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](Bulkdensity)
### Bulk density
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#BulkDensity`
Description | Bulk density of fresh concrete in kg/m3
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](ClassOfconcretemonitoring)
### Class Of concrete monitoring
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ClassOfMonitoring`
Description | Class Of concrete monitoring according to DIN EN 13670/DIN 1045-3 related to the properties of hardened concrete
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
[](Freshconcretetemperature)
### Fresh concrete temperature
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteTemperature`
Description | Fresh concrete temperature during testing of property in Celsius
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Storagecondition)
### Storage condition
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Condition`
Description | Description of storage condition
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Conversionfactor)
### Conversion factor
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConversionFactor`
Description | Conversion factor of compressive strength testing
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Dateofconcreting)
### Date of concreting
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DateOfConcreting`
Description | Date of concreting with format year-month-day in yyyy-mm-dd
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Dateofstripping)
### Date of stripping
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DateOfStripping`
Description | Date of stripping with format year-month-day in yyyy-mm-dd
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Deliverynote)
### Delivery note
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#DeliveryNote`
Description | Delivery note of mixed-ready concrete
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery) (c)<br />
Range(s) |[xsd:anyURI](http://www.w3.org/2001/XMLSchema#anyURI) (c)<br />
[](Storageduration)
### Storage duration
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Duration`
Description | Duration of storage in day
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Enddateofconcretecuring)
### End date of concrete curing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EndDate`
Description | End date of concrete curing with format year-month-day in yyyy-mm-dd
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Endtimeofpaving)
### End time of paving
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EndTimeOfPlacement`
Description | End time of paving with format hour-minute-second in hh-mm-ss
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteDelivery) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](Evaluationofthemeanvalue)
### Evaluation of the mean value
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#EvaluationOfTest`
Description | Evaluation of the mean value of the test in N/mm2
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Resultofcompressivestrength)
### Result of compressive strength
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FinalCompressiveStrength`
Description | Result of the compressive strength of the respective test sample  with consideration of the conversion factor in N/mm2
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Freshconcretetemperaturebeforeconcreting)
### Fresh concrete temperature before concreting
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteTemperature`
Description | Fresh concrete temperature before concreting in Celsius
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Heightofsample)
### Height of sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Height`
Description | Height of a test sample as cube in mm
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Storagehumidity)
### Storage humidity
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Humidity`
Description | Humidity of storage condition in %
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Intermediateresultofcompressivestrength)
### Intermediate result of compressive strength
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#InterimCompressiveStrength`
Description | Intermediate result of the compressive strength of the respective sample without conversion factor of in N/mm2
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Lengthofsample)
### Length of sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Length`
Description | Length of a test sample for cube in mm
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Maturityofconcrete)
### Maturity of concrete
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MaturityOfConcrete`
Description | Maturity of concrete in minute
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Maxtemperature)
### Max temperature
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MaxAirTemperature`
Description | Maximum temperature during post-treatment in Celsius
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Methodofconcretecuring)
### Method of concrete curing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MethodOfAftertreatment`
Description | Description of the method for concrete curing
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Mintemperature)
### Min temperature
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#MinAirTemperature`
Description | Minimum temperature during post-treatment in Celsius
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcreteCuring) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Teststandard)
### Test standard
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#NormativeReference`
Description | Norm or standard of the test method
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Temperatureofsample)
### Temperature of sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ObjectTemperature`
Description | Temperature of a test sample in Celsius
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Quantityofconcrete)
### Quantity of concrete
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#QuantityOfConcrete`
Description | Quantity of the concrete placement in cubature m3
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Rateofflowtabletest)
### Rate of flow table test
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#RateOfFlowTableTest`
Description | Rate of flow table test according to DIN EN 12350-5 in mm
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](SampleID)
### Sample ID
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SampleID`
Description | Name or ID of the test sample
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Dateofsampling)
### Date of sampling
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#SamplingDate`
Description | Date of sampling with format year-month-day in yyyy-mm-dd
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Storagetemperature)
### Storage temperature
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Temperature`
Description | Storage temperature in Celsius
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Storage) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Testedproperty)
### Tested property
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestCharacteristic`
Description | The property has to be tested
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Dateoftesting)
### Date of testing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestDate`
Description | Date of testing with format year-month-day in yyyy-mm-dd
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Testreport)
### Test report
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestReport`
Description | Report of conformity test of compressive strength
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[xsd:anyURI](http://www.w3.org/2001/XMLSchema#anyURI) (c)<br />
[](Timeoftesting)
### Time of testing
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestTime`
Description | Time of testing with format year-month-day in yyyy-mm-ddThh-mm-ss
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c)<br />
Range(s) |[xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br />
[](Typeoftest)
### Type of test
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestType`
Description | Type of test as self-inspection or third-party monitoring
Domain(s) |([http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConcretePlacement) (c) or [http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Test) (c))<br />
[](Valueofbreakingload)
### Value of breaking load
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestedBreakingLoad`
Description | Value of breaking load in N
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Densityofsample)
### Density of sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestedDensity`
Description | Density of a sample in kg/m3
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#ConformityOfCompressiveStrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Voidsratio)
### Voids ratio
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#VoidsRatio`
Description | Voids ratio of fresh concrete in V-%
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#FreshConcreteProperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Weigthofsample)
### Weigth of sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#Weigth`
Description | Weigth of a test sample in kg
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Widthordiameterofsample)
### Width or diameter of sample
Property | Value
--- | ---
IRI | `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#WidthOrDia`
Description | Width of a test sample as cube or diameter of a test sample as cylinder in mm
Domain(s) |[http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample](http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring#TestSample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />

## Named Individuals
## Namespaces
* **default (:)**
  * `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring/`
* **bcom**
  * `http://www.inf.bi.rub.de/semweb/ns/buildingconcretemonitoring/`
* **dc**
  * `http://purl.org/dc/terms/`
* **foaf**
  * `http://xmlns.com/foaf/0.1/`
* **owl**
  * `http://www.w3.org/2002/07/owl#`
* **prov**
  * `http://www.w3.org/ns/prov#`
* **rdf**
  * `http://www.w3.org/1999/02/22-rdf-syntax-ns#`
* **rdfs**
  * `http://www.w3.org/2000/01/rdf-schema#`
* **sdo**
  * `https://schema.org/`
* **skos**
  * `http://www.w3.org/2004/02/skos/core#`
* **vcard**
  * `http://www.w3.org/2006/vcard/ns#`
* **xml**
  * `http://www.w3.org/XML/1998/namespace`
* **xsd**
  * `http://www.w3.org/2001/XMLSchema#`

## Legend
* Classes: c
* Object Properties: op
* Functional Properties: fp
* Data Properties: dp
* Annotation Properties: dp
* Properties: p
* Named Individuals: ni