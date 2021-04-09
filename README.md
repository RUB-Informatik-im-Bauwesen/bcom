Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# Building Concrete Monitoring Ontology (BCOM)

## Metadata
* **IRI**
  * `https://w3id.org/bcom`
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
  * RDF ([BuildingConcreteMonitoring.jsonld](jsonld))
  * RDF ([BuildingConcreteMonitoring.nt](n-triples))
  * RDF ([BuildingConcreteMonitoring.rdf](rdf/xml))
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
IRI | `https://w3id.org/bcom#ConcreteCuring`
Description | <p>This class provides the necessary information of concrete curing after concreting</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:MethodOfAftertreatment](Methodofconcretecuring) (dp)<br />[bcom:EndDate](Enddateofconcretecuring) (dp)<br />[bcom:MaxAirTemperature](Maxtemperature) (dp)<br />[bcom:HasConcretePlacement](CuringhasConcreteWork) (op)<br />[bcom:BeginDate](Begindateofconcretecuring) (dp)<br />[bcom:MinAirTemperature](Mintemperature) (dp)<br />
In range of |[bcom:HasCuring](hasCuring) (op)<br />
### Concrete delivery
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcreteDelivery`
Description | <p>This class provides information about the delivery of concrete</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:EndTimeOfPlacement](Endtimeofpaving) (dp)<br />[bcom:BeginTimeOfPlacement](Begintimeofpaving) (dp)<br />[bcom:DeliveryNote](Deliverynote) (dp)<br />[bcom:DeliversConcreteFor](Deliversconcretefor) (op)<br />[bcom:HasSupplier](HasSupplier) (op)<br />
In range of |[bcom:HasDelivery](hasConcreteSupplier) (op)<br />
### Concrete placement
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcretePlacement`
Description | <p>This class provides the necessary information of current concreting of the construction</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:HasCuring](hasCuring) (op)<br />[bcom:DateOfConcreting](Dateofconcreting) (dp)<br />[bcom:DateOfStripping](Dateofstripping) (dp)<br />[bcom:QuantityOfConcrete](Quantityofconcrete) (dp)<br />[bcom:HasDelivery](hasConcreteSupplier) (op)<br />[bcom:FreshConcreteTemperature](Freshconcretetemperaturebeforeconcreting) (dp)<br />[bcom:ClassOfMonitoring](ClassOfconcretemonitoring) (dp)<br />
In range of |[bcom:HasConcretePlacement](CuringhasConcreteWork) (op)<br />[bcom:SuppliesConcreteTo](suppliesConcreteto) (op)<br />[bcom:DeliversConcreteFor](Deliversconcretefor) (op)<br />
### Conformity testing of compressive strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConformityOfCompressiveStrength`
Description | <p>This class provides the necessary information to perform and evaluate the conformity testing of concrete compressive strength.</p>
Super-classes |[bcom:Test](Test) (c)<br />
In domain of |[bcom:TestedBreakingLoad](Valueofbreakingload) (dp)<br />[bcom:InterimCompressiveStrength](Intermediateresultofcompressivestrength) (dp)<br />[bcom:TestedDensity](Densityofsample) (dp)<br />[bcom:TestCharacteristic](Testedproperty) (dp)<br />[bcom:EvaluationOfTest](Evaluationofthemeanvalue) (dp)<br />[bcom:ConversionFactor](Conversionfactor) (dp)<br />[bcom:NormativeReference](Teststandard) (dp)<br />[bcom:FinalCompressiveStrength](Resultofcompressivestrength) (dp)<br />
In range of |[bcom:HasTest](hasTestOfCompressiveStrength) (op)<br />
### Fresh concrete property testing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#FreshConcreteProperties`
Description | <p>This class represents a group of fresh concrete property.  A fresh concrete property set object will usually contain density, voids ratio, consistency.</p>
Super-classes |[bcom:Test](Test) (c)<br />
In domain of |[bcom:ConcreteTemperature](Freshconcretetemperature) (dp)<br />[bcom:BulkDensity](Bulkdensity) (dp)<br />[bcom:VoidsRatio](Voidsratio) (dp)<br />[bcom:RateOfFlowTableTest](Rateofflowtabletest) (dp)<br />[bcom:MaturityOfConcrete](Maturityofconcrete) (dp)<br />
### Storage of a test sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Storage`
Description | <p>This class represents the storage conditions of a test sample</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:Temperature](Storagetemperature) (dp)<br />[bcom:Humidity](Storagehumidity) (dp)<br />[bcom:Condition](Storagecondition) (dp)<br />[bcom:Duration](Storageduration) (dp)<br />[bcom:StoresSample](StoresSample) (op)<br />
In range of |[bcom:HasStorage](HasStorage) (op)<br />
### Test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Test`
Description | <p>Represents the super-class for different types of tests for placed concrete</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[bcom:FreshConcreteProperties](Freshconcretepropertytesting) (c)<br />[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
In domain of |[bcom:TestTime](Timeoftesting) (dp)<br />[bcom:HasTestSample](hasTestSample) (op)<br />[bcom:HasTestPerson](hasPerformTestPerson) (op)<br />[bcom:HasTest](hasTestOfCompressiveStrength) (op)<br />[bcom:TestReport](Testreport) (dp)<br />[bcom:HasTestOrganisation](hasPerformTestOrganisation) (op)<br />[bcom:TestDate](Dateoftesting) (dp)<br />
In range of |[bcom:HasTestSubjects](hasTestSubjects) (op)<br />
### Test sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestSample`
Description | <p>This class provides the information of test sample for conformity test of concrete compressive strength</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:Weigth](Weigthofsample) (dp)<br />[bcom:WidthOrDia](Widthordiameterofsample) (dp)<br />[bcom:Length](Lengthofsample) (dp)<br />[bcom:HasStorage](HasStorage) (op)<br />[bcom:Height](Heightofsample) (dp)<br />[bcom:ObjectTemperature](Temperatureofsample) (dp)<br />[bcom:SamplingDate](Dateofsampling) (dp)<br />[bcom:SampleID](SampleID) (dp)<br />
In range of |[bcom:StoresSample](StoresSample) (op)<br />[bcom:HasTestSample](hasTestSample) (op)<br />

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
IRI | `https://w3id.org/bcom#DeliversConcreteFor`
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](CuringhasConcreteWork)
### Curing has Concrete Work
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasConcretePlacement`
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](hasCuring)
### has Curing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasCuring`
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
[](hasConcreteSupplier)
### has Concrete Supplier
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasDelivery`
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
[](HasStorage)
### HasStorage
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasStorage`
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[bcom:Storage](Storageofatestsample) (c)<br />
[](HasSupplier)
### has Concrete Supplier
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasSupplier`
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
[](hasTestOfCompressiveStrength)
### has Test Of Compressive Strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTest`
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
[](hasPerformTestOrganisation)
### has Perform Test Organisation
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestOrganisation`
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
[](hasPerformTestPerson)
### has Perform Test Person
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestPerson`
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[vcard:Individual](http://www.w3.org/2006/vcard/ns#Individual) (c)<br />
[](hasTestSample)
### has Test Sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestSample`
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[bcom:TestSample](Testsample) (c)<br />
[](hasTestSubjects)
### has Test Subjects
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestSubjects`
Domain(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
Range(s) |[bcom:Test](Test) (c)<br />
[](StoresSample)
### StoresSample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#StoresSample`
Domain(s) |[bcom:Storage](Storageofatestsample) (c)<br />
Range(s) |[bcom:TestSample](Testsample) (c)<br />
[](suppliesConcreteto)
### supplies Concrete to
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#SuppliesConcreteTo`
Domain(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />

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
IRI | `https://w3id.org/bcom#AirTemperature`
Description | Air temperature during concreting or test on fresh concrete in Celsius
Domain(s) |([bcom:ConcretePlacement](Concreteplacement) (c) or [bcom:TestSample](Testsample) (c))<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Begindateofconcretecuring)
### Begin date of concrete curing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#BeginDate`
Description | Begin date of concrete curing with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Begintimeofpaving)
### Begin time of paving
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#BeginTimeOfPlacement`
Description | Begin time of paving with format hour-minute-second in hh-mm-ss
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](Bulkdensity)
### Bulk density
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#BulkDensity`
Description | Bulk density of fresh concrete in kg/m3
Domain(s) |[bcom:FreshConcreteProperties](Freshconcretepropertytesting) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](ClassOfconcretemonitoring)
### Class Of concrete monitoring
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ClassOfMonitoring`
Description | Class Of concrete monitoring according to DIN EN 13670/DIN 1045-3 related to the properties of hardened concrete
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](Freshconcretetemperature)
### Fresh concrete temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcreteTemperature`
Description | Fresh concrete temperature during testing of property in Celsius
Domain(s) |[bcom:FreshConcreteProperties](Freshconcretepropertytesting) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Storagecondition)
### Storage condition
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Condition`
Description | Description of storage condition
Domain(s) |[bcom:Storage](Storageofatestsample) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Conversionfactor)
### Conversion factor
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConversionFactor`
Description | Conversion factor of compressive strength testing
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Dateofconcreting)
### Date of concreting
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DateOfConcreting`
Description | Date of concreting with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Dateofstripping)
### Date of stripping
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DateOfStripping`
Description | Date of stripping with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Deliverynote)
### Delivery note
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DeliveryNote`
Description | Delivery note of mixed-ready concrete
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[xsd:anyURI](http://www.w3.org/2001/XMLSchema#anyURI) (c)<br />
[](Storageduration)
### Storage duration
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Duration`
Description | Duration of storage in day
Domain(s) |[bcom:Storage](Storageofatestsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Enddateofconcretecuring)
### End date of concrete curing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#EndDate`
Description | End date of concrete curing with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Endtimeofpaving)
### End time of paving
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#EndTimeOfPlacement`
Description | End time of paving with format hour-minute-second in hh-mm-ss
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](Evaluationofthemeanvalue)
### Evaluation of the mean value
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#EvaluationOfTest`
Description | Evaluation of the mean value of the test in N/mm2
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Resultofcompressivestrength)
### Result of compressive strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#FinalCompressiveStrength`
Description | Result of the compressive strength of the respective test sample  with consideration of the conversion factor in N/mm2
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Freshconcretetemperaturebeforeconcreting)
### Fresh concrete temperature before concreting
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#FreshConcreteTemperature`
Description | Fresh concrete temperature before concreting in Celsius
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Heightofsample)
### Height of sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Height`
Description | Height of a test sample as cube in mm
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Storagehumidity)
### Storage humidity
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Humidity`
Description | Humidity of storage condition in %
Domain(s) |[bcom:Storage](Storageofatestsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Intermediateresultofcompressivestrength)
### Intermediate result of compressive strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#InterimCompressiveStrength`
Description | Intermediate result of the compressive strength of the respective sample without conversion factor of in N/mm2
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Lengthofsample)
### Length of sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Length`
Description | Length of a test sample for cube in mm
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Maturityofconcrete)
### Maturity of concrete
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MaturityOfConcrete`
Description | Maturity of concrete in minute
Domain(s) |[bcom:FreshConcreteProperties](Freshconcretepropertytesting) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Maxtemperature)
### Max temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MaxAirTemperature`
Description | Maximum temperature during post-treatment in Celsius
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Methodofconcretecuring)
### Method of concrete curing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MethodOfAftertreatment`
Description | Description of the method for concrete curing
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Mintemperature)
### Min temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MinAirTemperature`
Description | Minimum temperature during post-treatment in Celsius
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Teststandard)
### Test standard
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#NormativeReference`
Description | Norm or standard of the test method
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Temperatureofsample)
### Temperature of sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ObjectTemperature`
Description | Temperature of a test sample in Celsius
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Quantityofconcrete)
### Quantity of concrete
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#QuantityOfConcrete`
Description | Quantity of the concrete placement in cubature m3
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Rateofflowtabletest)
### Rate of flow table test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#RateOfFlowTableTest`
Description | Rate of flow table test according to DIN EN 12350-5 in mm
Domain(s) |[bcom:FreshConcreteProperties](Freshconcretepropertytesting) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](SampleID)
### Sample ID
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#SampleID`
Description | Name or ID of the test sample
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Dateofsampling)
### Date of sampling
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#SamplingDate`
Description | Date of sampling with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Storagetemperature)
### Storage temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Temperature`
Description | Storage temperature in Celsius
Domain(s) |[bcom:Storage](Storageofatestsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Testedproperty)
### Tested property
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestCharacteristic`
Description | The property has to be tested
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](Dateoftesting)
### Date of testing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestDate`
Description | Date of testing with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](Testreport)
### Test report
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestReport`
Description | Report of conformity test of compressive strength
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[xsd:anyURI](http://www.w3.org/2001/XMLSchema#anyURI) (c)<br />
[](Timeoftesting)
### Time of testing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestTime`
Description | Time of testing with format year-month-day in yyyy-mm-ddThh-mm-ss
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br />
[](Typeoftest)
### Type of test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestType`
Description | Type of test as self-inspection or third-party monitoring
Domain(s) |([bcom:ConcretePlacement](Concreteplacement) (c) or [bcom:Test](Test) (c))<br />
[](Valueofbreakingload)
### Value of breaking load
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestedBreakingLoad`
Description | Value of breaking load in N
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Densityofsample)
### Density of sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestedDensity`
Description | Density of a sample in kg/m3
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Voidsratio)
### Voids ratio
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#VoidsRatio`
Description | Voids ratio of fresh concrete in V-%
Domain(s) |[bcom:FreshConcreteProperties](Freshconcretepropertytesting) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Weigthofsample)
### Weigth of sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Weigth`
Description | Weigth of a test sample in kg
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](Widthordiameterofsample)
### Width or diameter of sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#WidthOrDia`
Description | Width of a test sample as cube or diameter of a test sample as cylinder in mm
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />

## Named Individuals
## Namespaces
* **default (:)**
  * `https://w3id.org/bcom#`
* **bcom**
  * `https://w3id.org/bcom#`
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