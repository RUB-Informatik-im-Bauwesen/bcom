Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# Building Concrete Monitoring Ontology (BCOM) [![DOI](https://zenodo.org/badge/332699346.svg)](https://zenodo.org/badge/latestdoi/332699346)

## Metadata
* **IRI**
  * `https://w3id.org/bcom`
* **Publisher(s)**
  * Chair of Computing in Engineering, Ruhr University Bochum
* **Creators(s)**
  * Liu Liu, Ruhr University Bochum
  * Philipp Hagedorn, Ruhr University Bochum
* **Created**
  * 2021-01-20
* **Modified**
  * 2021-07-21
* **Issued**
  * 2021-01-20
* **Version Information**
  * 0.3
* **License &amp; Rights**
  * [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
  * &copy; 2021 by Chair of Computing in Engineering, Ruhr University Bochum
* **Source**
  * [https://github.com/RUB-Informatik-im-Bauwesen/bcom](https://github.com/RUB-Informatik-im-Bauwesen/bcom)
* **Ontology RDF**
  * RDF ([BuildingConcreteMonitoring.ttl](turtle))
  * RDF ([BuildingConcreteMonitoring.jsonld](jsonld))
  * RDF ([BuildingConcreteMonitoring.nt](n-triples))
  * RDF ([BuildingConcreteMonitoring.rdf](rdf/xml))
### Description
<p>The Building Concrete Monitoring Ontology (BCOM) is defined for capturing information of concrete work, concrete curing and testing of concrete properties. Further Information on the development and usage of the Ontology can be found in the following publication: Liu et al. (2021): An ontology integrating as-built information for infrastructure asset management using BIM and semantic web. In: Proceedings of 2021 European Conference on Computing in Construction, Online eConference, URL: https://ec-3.org/publications/conferences/2021/paper/?id=167</p>

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
[Fresh concrete properties](#Freshconcreteproperties),
[Storage](#Storage),
[Test](#Test),
[Test sample](#Testsample),
### Concrete curing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcreteCuring`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class provides information about the curing process after a concrete placement.</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:MinAirTemperature](minairtemperature) (dp)<br />[bcom:MaxAirTemperature](maxairtemperature) (dp)<br />[bcom:HasConcretePlacement](hasconcreteplacement) (op)<br />[bcom:EndDate](enddate) (dp)<br />[bcom:BeginDate](begindate) (dp)<br />[bcom:MethodOfAftertreatment](methodofaftertreatment) (dp)<br />
In range of |[bcom:HasCuring](hascuring) (op)<br />
### Concrete delivery
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcreteDelivery`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class provides information about a concrete delivery.</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:BeginTimeOfPlacement](begintime) (dp)<br />[bcom:DeliveryNote](deliverynote) (dp)<br />[bcom:EndTimeOfPlacement](endtimeofplacement) (dp)<br />[bcom:DeliversConcreteFor](deliversconcretefor) (op)<br />[bcom:HasSupplier](hassupplier) (op)<br />
In range of |[bcom:HasDelivery](hasdelivery) (op)<br />
### Concrete placement
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcretePlacement`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class provides information about a concreting process itself.</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:QuantityOfConcrete](quantityofconcrete) (dp)<br />[bcom:HasCuring](hascuring) (op)<br />[bcom:DateOfConcreting](dateofconcreting) (dp)<br />[bcom:HasDelivery](hasdelivery) (op)<br />[bcom:HasTest](hastest) (op)<br />[bcom:DateOfStripping](dateofstripping) (dp)<br />[bcom:ClassOfMonitoring](classofmonitoring) (dp)<br />[bcom:FreshConcreteTemperature](FreshConcreteTemperature) (dp)<br />
In range of |[bcom:SuppliesConcreteTo](suppliesconcreteto) (op)<br />[bcom:IsTestOf](istestof) (op)<br />[bcom:DeliversConcreteFor](deliversconcretefor) (op)<br />[bcom:HasConcretePlacement](hasconcreteplacement) (op)<br />
### Conformity testing of compressive strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConformityOfCompressiveStrength`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class provides information needed for performing and evaluating the conformity of concrete compressive strength.</p>
Super-classes |[bcom:Test](Test) (c)<br />
In domain of |[bcom:EvaluationOfTest](evaluationoftest) (dp)<br />[bcom:InterimCompressiveStrength](intermediatecompressivestrength) (dp)<br />[bcom:ConversionFactor](conversionfactor) (dp)<br />[bcom:TestedDensity](testeddensity) (dp)<br />[bcom:NormativeReference](normativereference) (dp)<br />[bcom:TestCharacteristic](testedcharacteristic) (dp)<br />[bcom:FinalCompressiveStrength](finalcompressivestrength) (dp)<br />[bcom:TestedBreakingLoad](testedbreakingload) (dp)<br />
### Fresh concrete properties
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#FreshConcreteProperties`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class represents a group of fresh concrete properties.  A fresh concrete propertyset object will usually contain density, voids ratio, consistency.</p>
Super-classes |[bcom:Test](Test) (c)<br />
In domain of |[bcom:MaturityOfConcrete](maturityofconcrete) (dp)<br />[bcom:VoidsRatio](voidsratio) (dp)<br />[bcom:ConcreteTemperature](freshconcretetemperature) (dp)<br />[bcom:BulkDensity](bulkdensity) (dp)<br />[bcom:RateOfFlowTableTest](rateofflowtabletest) (dp)<br />
### Storage
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Storage`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class represents the storage conditions of a test sample.</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:Humidity](humidity) (dp)<br />[bcom:Temperature](temperature) (dp)<br />[bcom:Condition](storagecondition) (dp)<br />[bcom:StoresSample](storessample) (op)<br />[bcom:Duration](duration) (dp)<br />
In range of |[bcom:HasStorage](hasstorage) (op)<br />
### Test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Test`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class represents the super-class for different types of tests, that can be performed on placed concrete.</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
Sub-classes |[bcom:FreshConcreteProperties](Freshconcreteproperties) (c)<br />[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
In domain of |[bcom:TestTime](testtime) (dp)<br />[bcom:HasTestPerson](hastestperson) (op)<br />[bcom:IsTestOf](istestof) (op)<br />[bcom:TestReport](testreport) (dp)<br />[bcom:HasTestSample](hastestsample) (op)<br />[bcom:TestDate](testdate) (dp)<br />[bcom:HasTestOrganisation](hastestorganisation) (op)<br />
In range of |[bcom:HasTest](hastest) (op)<br />[bcom:IsTestOrganisationOf](istestorganisationof) (op)<br />[bcom:IsTestSampleOf](istestsampleof) (op)<br />[bcom:IsTestPersonOf](istestpersonof) (op)<br />
### Test sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestSample`
Is Defined By | https://w3id.org/bcom#
Description | <p>This class provides information about test samples.</p>
Super-classes |[owl:Thing](http://www.w3.org/2002/07/owl#Thing) (c)<br />
In domain of |[bcom:Height](height) (dp)<br />[bcom:SamplingDate](samplingdate) (dp)<br />[bcom:HasStorage](hasstorage) (op)<br />[bcom:IsTestSampleOf](istestsampleof) (op)<br />[bcom:WidthOrDia](widthordia) (dp)<br />[bcom:ObjectTemperature](objecttemperature) (dp)<br />[bcom:SampleID](sampleID) (dp)<br />[bcom:Length](length) (dp)<br />[bcom:Weigth](weigth) (dp)<br />
In range of |[bcom:StoresSample](storessample) (op)<br />[bcom:HasTestSample](hastestsample) (op)<br />

## Object Properties
[delivers concrete for](#deliversconcretefor),
[has concrete placement](#hasconcreteplacement),
[has curing](#hascuring),
[has delivery](#hasdelivery),
[has storage](#hasstorage),
[has supplier](#hassupplier),
[has test](#hastest),
[has test organisation](#hastestorganisation),
[has test person](#hastestperson),
[has test sample](#hastestsample),
[is test of](#istestof),
[is test organisation of](#istestorganisationof),
[is test person of](#istestpersonof),
[is test sample of](#istestsampleof),
[stores sample](#storessample),
[supplies concrete to](#suppliesconcreteto),
[](deliversconcretefor)
### delivers concrete for
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DeliversConcreteFor`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete delivery to its concrete placement activity where it was used for.
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](hasconcreteplacement)
### has concrete placement
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasConcretePlacement`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete curing process to its concrete placement activity.
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](hascuring)
### has curing
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasCuring`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete placement activity to its curing process.
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
[](hasdelivery)
### has delivery
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasDelivery`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete placement activity to its concrete delivery providing the used concrete.
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
[](hasstorage)
### has storage
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasStorage`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete test sample to its storage details.
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[bcom:Storage](Storage) (c)<br />
[](hassupplier)
### has supplier
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasSupplier`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete delivery to its supplier.
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
[](hastest)
### has test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTest`
Is Defined By | https://w3id.org/bcom#
Description | This property links a concrete placement activity to its test procedure.
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[bcom:Test](Test) (c)<br />
[](hastestorganisation)
### has test organisation
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestOrganisation`
Is Defined By | https://w3id.org/bcom#
Description | This property links a test procedure to its organization which is performing the test.
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
[](hastestperson)
### has test person
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestPerson`
Is Defined By | https://w3id.org/bcom#
Description | This property links a test procedure to its person who is performing the test.
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[vcard:Individual](http://www.w3.org/2006/vcard/ns#Individual) (c)<br />
[](hastestsample)
### has test sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#HasTestSample`
Is Defined By | https://w3id.org/bcom#
Description | This property links a test procedure to its test samples tested within this procedure.
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[bcom:TestSample](Testsample) (c)<br />
[](istestof)
### is test of
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#IsTestOf`
Is Defined By | https://w3id.org/bcom#
Description | This property links a test procedure to its concrete placement activity whithin its test samples have been concreted.
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](istestorganisationof)
### is test organisation of
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#IsTestOrganisationOf`
Is Defined By | https://w3id.org/bcom#
Description | This property links an organization to its test procedures that have been performed by itself.
Domain(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
Range(s) |[bcom:Test](Test) (c)<br />
[](istestpersonof)
### is test person of
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#IsTestPersonOf`
Is Defined By | https://w3id.org/bcom#
Description | This property links a test examining person to its test procedures that have been performed by itslef.
Domain(s) |[vcard:Individual](http://www.w3.org/2006/vcard/ns#Individual) (c)<br />
Range(s) |[bcom:Test](Test) (c)<br />
[](istestsampleof)
### is test sample of
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#IsTestSampleOf`
Is Defined By | https://w3id.org/bcom#
Description | This property links a test sample to its test procedure within which it has been tested.
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[bcom:Test](Test) (c)<br />
[](storessample)
### stores sample
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#StoresSample`
Is Defined By | https://w3id.org/bcom#
Description | This property links storage details to its test samples that has been stored under the specific storage conditions.
Domain(s) |[bcom:Storage](Storage) (c)<br />
Range(s) |[bcom:TestSample](Testsample) (c)<br />
[](suppliesconcreteto)
### supplies concrete to
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#SuppliesConcreteTo`
Is Defined By | https://w3id.org/bcom#
Description | This property links an organization to its concrete placement activities where it delivered concrete for.
Domain(s) |[vcard:Organization](http://www.w3.org/2006/vcard/ns#Organization) (c)<br />
Range(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />

## Datatype Properties
[air temperature](#airtemperature),
[begin date](#begindate),
[begin time](#begintime),
[bulk density](#bulkdensity),
[class of monitoring](#classofmonitoring),
[fresh concrete temperature](#freshconcretetemperature),
[storage condition](#storagecondition),
[conversion factor](#conversionfactor),
[date of concreting](#dateofconcreting),
[date of stripping](#dateofstripping),
[delivery note](#deliverynote),
[duration](#duration),
[end date](#enddate),
[end time of placement](#endtimeofplacement),
[evaluation of test](#evaluationoftest),
[final compressive strength](#finalcompressivestrength),
[fresh concrete temperature](#FreshConcreteTemperature),
[height](#height),
[humidity](#humidity),
[intermediate compressive strength](#intermediatecompressivestrength),
[length](#length),
[maturity of concrete](#maturityofconcrete),
[max air temperature](#maxairtemperature),
[method of aftertreatment](#methodofaftertreatment),
[min air temperature](#minairtemperature),
[normative reference](#normativereference),
[object temperature](#objecttemperature),
[quantity of concrete](#quantityofconcrete),
[rate of flow table test](#rateofflowtabletest),
[sample ID](#sampleID),
[sampling date](#samplingdate),
[temperature](#temperature),
[tested characteristic](#testedcharacteristic),
[test date](#testdate),
[test report](#testreport),
[test time](#testtime),
[test type](#testtype),
[tested breaking load](#testedbreakingload),
[tested density](#testeddensity),
[voids ratio](#voidsratio),
[weigth](#weigth),
[width or dia](#widthordia),
[](airtemperature)
### air temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#AirTemperature`
Is Defined By | https://w3id.org/bcom#
Description | air temperature during concreting or testing on fresh concrete in degree Celsius
Domain(s) |([bcom:ConcretePlacement](Concreteplacement) (c) or [bcom:TestSample](Testsample) (c))<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](begindate)
### begin date
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#BeginDate`
Is Defined By | https://w3id.org/bcom#
Description | begin date of concrete curing with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](begintime)
### begin time
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#BeginTimeOfPlacement`
Is Defined By | https://w3id.org/bcom#
Description | begin time of concrete placement with format hour-minute-second in hh:mm:ss
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](bulkdensity)
### bulk density
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#BulkDensity`
Is Defined By | https://w3id.org/bcom#
Description | bulk density of fresh concrete in kg/m^3
Domain(s) |[bcom:FreshConcreteProperties](Freshconcreteproperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](classofmonitoring)
### class of monitoring
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ClassOfMonitoring`
Is Defined By | https://w3id.org/bcom#
Description | class of concrete monitoring according to DIN EN 13670 / DIN 1045-3 related to the properties of hardened concrete
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
[](freshconcretetemperature)
### fresh concrete temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConcreteTemperature`
Is Defined By | https://w3id.org/bcom#
Description | fresh concrete temperature during testing of properties in degree Celsius
Domain(s) |[bcom:FreshConcreteProperties](Freshconcreteproperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](storagecondition)
### storage condition
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Condition`
Is Defined By | https://w3id.org/bcom#
Description | description of storage conditions
Domain(s) |[bcom:Storage](Storage) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](conversionfactor)
### conversion factor
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ConversionFactor`
Is Defined By | https://w3id.org/bcom#
Description | conversion factor of compressive strength testing
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](dateofconcreting)
### date of concreting
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DateOfConcreting`
Is Defined By | https://w3id.org/bcom#
Description | date of concreting with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](dateofstripping)
### date of stripping
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DateOfStripping`
Is Defined By | https://w3id.org/bcom#
Description | date of stripping with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](deliverynote)
### delivery note
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#DeliveryNote`
Is Defined By | https://w3id.org/bcom#
Description | delivery note of mixed-ready concrete
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[xsd:anyURI](http://www.w3.org/2001/XMLSchema#anyURI) (c)<br />
[](duration)
### duration
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Duration`
Is Defined By | https://w3id.org/bcom#
Description | duration of  storage for test sample in days
Domain(s) |[bcom:Storage](Storage) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](enddate)
### end date
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#EndDate`
Is Defined By | https://w3id.org/bcom#
Description | end date of concrete curing with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](endtimeofplacement)
### end time of placement
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#EndTimeOfPlacement`
Is Defined By | https://w3id.org/bcom#
Description | end time of concrete placement with format hour-minute-second in hh:mm:ss
Domain(s) |[bcom:ConcreteDelivery](Concretedelivery) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](evaluationoftest)
### evaluation of test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#EvaluationOfTest`
Is Defined By | https://w3id.org/bcom#
Description | evaluation of the mean value of the test in N/mm^2
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](finalcompressivestrength)
### final compressive strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#FinalCompressiveStrength`
Is Defined By | https://w3id.org/bcom#
Description | result of the compressive strength of the respective test sample under consideration of the conversion factor in N/mm^2
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](FreshConcreteTemperature)
### fresh concrete temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#FreshConcreteTemperature`
Is Defined By | https://w3id.org/bcom#
Description | fresh concrete temperature before concrete placement in degree Celsius
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](height)
### height
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Height`
Is Defined By | https://w3id.org/bcom#
Description | height of a test sample as cube or as cylinder in mm
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](humidity)
### humidity
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Humidity`
Is Defined By | https://w3id.org/bcom#
Description | relative humidity of storage condition in %
Domain(s) |[bcom:Storage](Storage) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](intermediatecompressivestrength)
### intermediate compressive strength
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#InterimCompressiveStrength`
Is Defined By | https://w3id.org/bcom#
Description | intermediate result of the compressive strength of the respective sample without conversion factor of in N/mm^2
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](length)
### length
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Length`
Is Defined By | https://w3id.org/bcom#
Description | length of a test sample for cubes in mm
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](maturityofconcrete)
### maturity of concrete
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MaturityOfConcrete`
Is Defined By | https://w3id.org/bcom#
Description | maturity of concrete in minutes
Domain(s) |[bcom:FreshConcreteProperties](Freshconcreteproperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](maxairtemperature)
### max air temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MaxAirTemperature`
Is Defined By | https://w3id.org/bcom#
Description | maximum air temperature during post-treatment in degree Celsius
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](methodofaftertreatment)
### method of aftertreatment
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MethodOfAftertreatment`
Is Defined By | https://w3id.org/bcom#
Description | description for the method of concrete curing
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](minairtemperature)
### min air temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#MinAirTemperature`
Is Defined By | https://w3id.org/bcom#
Description | minimum air temperature during post-treatment in degree Celsius
Domain(s) |[bcom:ConcreteCuring](Concretecuring) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](normativereference)
### normative reference
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#NormativeReference`
Is Defined By | https://w3id.org/bcom#
Description | norm or standard of the test method
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](objecttemperature)
### object temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#ObjectTemperature`
Is Defined By | https://w3id.org/bcom#
Description | object temperature of a test sample in degree Celsius
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](quantityofconcrete)
### quantity of concrete
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#QuantityOfConcrete`
Is Defined By | https://w3id.org/bcom#
Description | quantity of the concrete placement in cubature m^3
Domain(s) |[bcom:ConcretePlacement](Concreteplacement) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](rateofflowtabletest)
### rate of flow table test
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#RateOfFlowTableTest`
Is Defined By | https://w3id.org/bcom#
Description | rate of flow table test according to DIN EN 12350-5 in mm
Domain(s) |[bcom:FreshConcreteProperties](Freshconcreteproperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](sampleID)
### sample ID
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#SampleID`
Is Defined By | https://w3id.org/bcom#
Description | name or ID of the test sample
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](samplingdate)
### sampling date
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#SamplingDate`
Is Defined By | https://w3id.org/bcom#
Description | date of sampling with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](temperature)
### temperature
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Temperature`
Is Defined By | https://w3id.org/bcom#
Description | storage temperature in degree Celsius
Domain(s) |[bcom:Storage](Storage) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](testedcharacteristic)
### tested characteristic
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestCharacteristic`
Is Defined By | https://w3id.org/bcom#
Description | the material property that has to be tested
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](testdate)
### test date
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestDate`
Is Defined By | https://w3id.org/bcom#
Description | date of testing with format year-month-day in yyyy-mm-dd
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[xsd:date](http://www.w3.org/2001/XMLSchema#date) (c)<br />
[](testreport)
### test report
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestReport`
Is Defined By | https://w3id.org/bcom#
Description | report of conformity test of concrete
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[xsd:anyURI](http://www.w3.org/2001/XMLSchema#anyURI) (c)<br />
[](testtime)
### test time
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestTime`
Is Defined By | https://w3id.org/bcom#
Description | time of testing with format hour-minute-second in hh:mm:ss
Domain(s) |[bcom:Test](Test) (c)<br />
Range(s) |[xsd:time](http://www.w3.org/2001/XMLSchema#time) (c)<br />
[](testtype)
### test type
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestType`
Is Defined By | https://w3id.org/bcom#
Description | type of test as self-inspection or third-party monitoring
Domain(s) |([bcom:ConcretePlacement](Concreteplacement) (c) or [bcom:Test](Test) (c))<br />
[](testedbreakingload)
### tested breaking load
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestedBreakingLoad`
Is Defined By | https://w3id.org/bcom#
Description | value of breaking load of test procedure in N
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](testeddensity)
### tested density
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#TestedDensity`
Is Defined By | https://w3id.org/bcom#
Description | value of density from a sample in kg/m^3
Domain(s) |[bcom:ConformityOfCompressiveStrength](Conformitytestingofcompressivestrength) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](voidsratio)
### voids ratio
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#VoidsRatio`
Is Defined By | https://w3id.org/bcom#
Description | voids ratio of fresh concrete in V-%
Domain(s) |[bcom:FreshConcreteProperties](Freshconcreteproperties) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](weigth)
### weigth
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#Weigth`
Is Defined By | https://w3id.org/bcom#
Description | weigth of a test sample in kg
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />
[](widthordia)
### width or dia
Property | Value
--- | ---
IRI | `https://w3id.org/bcom#WidthOrDia`
Is Defined By | https://w3id.org/bcom#
Description | width of a test sample as cube or diameter of a test sample as cylinder in mm
Domain(s) |[bcom:TestSample](Testsample) (c)<br />
Range(s) |[xsd:decimal](http://www.w3.org/2001/XMLSchema#decimal) (c)<br />

## Named Individuals
## Namespaces
* **default (:)**
  * `https://w3id.org/bcom#`
* **bcom**
  * `https://w3id.org/bcom#`
* **cc**
  * `http://creativecommons.org/ns#`
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
* **vann**
  * `http://purl.org/vocab/vann/`
* **vcard**
  * `http://www.w3.org/2006/vcard/ns#`
* **vs**
  * `http://www.w3.org/2003/06/sw-vocab-status/ns#`
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
