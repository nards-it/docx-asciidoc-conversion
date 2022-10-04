![](media/image2.jpeg){width="1.3715277777777777in" height="0.9444444444444444in"}

![](media/image3.wmf){width="0.9770833333333333in" height="0.9708333333333333in"}

INSPIRE\
Infrastructure for Spatial Information in Europe

D2.8.I.1 Data Specification on Coordinate Reference Systems -- Technical Guidelines

  ----------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Title**         D2.8.I.1 Data Specification on *Coordinate Reference Systems* -- Technical Guidelines
  **Creator**       INSPIRE Thematic Working Group Coordinate Reference Systems & Geographical Grid Systems
  **Date**          2014-04-15
  **Subject**       INSPIRE Data Specification for the spatial data theme *Coordinate Reference Systems*
  **Publisher**     INSPIRE Thematic Working Group Coordinate Reference Systems & Geographical Grid Systems
  **Type**          Text
  **Description**   This document describes the INSPIRE Data Specification for the spatial data theme *Coordinate Reference Systems*
  **Contributor**   Members of the INSPIRE Thematic Working Group Coordinate Reference Systems & Geographical Grid Systems
  **Format**        Portable Document Format (pdf)
  **Source**        
  **Rights**        Public
  **Identifier**    D2.8.I.1_v3.2
  **Language**      En
  **Relation**      Directive 2007/2/EC of the European Parliament and of the Council of 14 March 2007 establishing an Infrastructure for Spatial Information in the European Community (INSPIRE)
  **Coverage**      Project duration
  ----------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Foreword**

**How to read the document?**

This document describes the *"INSPIRE data specification on Coordinate Reference Systems -- Technical Guidelines"* version 3.2rc2 as developed by the Thematic Working Group (TWG) *INSPIRE Thematic Working Group Coordinate Reference Systems & Geographical Grid Systems* using both natural and a conceptual schema language.

The data specification is based on a common template[^1] used for all data specifications, which has been harmonised using the experience from the development of the Annex I, II and III data specifications.

This document provides guidelines for the implementation of the provisions laid down in the draft Implementing Rule for spatial data sets and services of the INSPIRE Directive. It also includes additional requirements and recommendations that, although not included in the Implementing Rule, are relevant to guarantee or to increase data interoperability.

Two executive summaries provide a quick overview of the INSPIRE data specification process in general, and the content of the data specification on *Coordinate Reference Systems* in particular. We highly recommend that managers, decision makers, and all those new to the INSPIRE process and/or information modelling should read these executive summaries first.

The UML diagrams (in Chapter 5) offer a rapid way to see the main elements of the specifications and their relationships. The definition of the spatial object types, attributes, and relationships are included in the Feature Catalogue (also in Chapter 5). People having thematic expertise but not familiar with UML can fully understand the content of the data model focusing on the Feature Catalogue. Users might also find the Feature Catalogue especially useful to check if it contains the data necessary for the applications that they run. The technical details are expected to be of prime interest to those organisations that are responsible for implementing INSPIRE within the field of *Coordinate Reference Systems*, but also to other stakeholders and users of the spatial data infrastructure.

The technical provisions and the underlying concepts are often illustrated by examples. Smaller examples are within the text of the specification, while longer explanatory examples and descriptions of selected use cases are attached in the annexes.

In order to distinguish the INSPIRE spatial data themes from the spatial object types, the INSPIRE spatial data themes are written in *italics.*

  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  The document will be publicly available as a 'non-paper'. It does not represent an official position of the European Commission, and as such cannot be invoked in the context of legal procedures.
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Legal Notice**

Neither the European Commission nor any person acting on behalf of the Commission is responsible for the use which might be made of this publication.

**Interoperability of Spatial Data Sets and Services --\
General Executive Summary**

The challenges regarding the lack of availability, quality, organisation, accessibility, and sharing of spatial information are common to a large number of policies and activities and are experienced across the various levels of public authority in Europe. In order to solve these problems it is necessary to take measures of coordination between the users and providers of spatial information. The Directive 2007/2/EC of the European Parliament and of the Council adopted on 14 March 2007 aims at establishing an Infrastructure for Spatial Information in the European Community (INSPIRE) for environmental policies, or policies and activities that have an impact on the environment.

INSPIRE is based on the infrastructures for spatial information that are created and maintained by the Member States. To support the establishment of a European infrastructure, Implementing Rules addressing the following components of the infrastructure have been specified: metadata, interoperability of spatial data sets (as described in Annexes I, II, III of the Directive) and spatial data services, network services, data and service sharing, and monitoring and reporting procedures.

INSPIRE does not require collection of new data. However, after the period specified in the Directive[^2] Member States have to make their data available according to the Implementing Rules.

Interoperability in INSPIRE means the possibility to combine spatial data and services from different sources across the European Community in a consistent way without involving specific efforts of humans or machines. It is important to note that "interoperability" is understood as providing access to spatial data sets through network services, typically via Internet. Interoperability may be achieved by either changing (harmonising) and storing existing data sets or transforming them via services for publication in the INSPIRE infrastructure. It is expected that users will spend less time and efforts on understanding and integrating data when they build their applications based on data delivered in accordance with INSPIRE.

In order to benefit from the endeavours of international standardisation bodies and organisations established under international law their standards and technical means have been utilised and referenced, whenever possible.

To facilitate the implementation of INSPIRE, it is important that all stakeholders have the opportunity to participate in specification and development. For this reason, the Commission has put in place a consensus building process involving data users, and providers together with representatives of industry, research and government. These stakeholders, organised through Spatial Data Interest Communities (SDIC) and Legally Mandated Organisations (LMO)[^3], have provided reference materials, participated in the user requirement and technical[^4] surveys, proposed experts for the Data Specification Drafting Team[^5], the Thematic Working Groups[^6] and other ad-hoc cross-thematic technical groups and participated in the public stakeholder consultations on draft versions of the data specifications. These consultations covered expert reviews as well as feasibility and fitness-for-purpose testing of the data specifications[^7].

This open and participatory approach was successfully used during the development of the data specifications on Annex I, II and III data themes as well as during the preparation of the Implementing Rule on Interoperability of Spatial Data Sets and Services[^8] for Annex I spatial data themes and of its amendment regarding the themes of Annex II and III.

The development framework elaborated by the Data Specification Drafting Team aims at keeping the data specifications of the different themes coherent. It summarises the methodology to be used for the development of the data specifications, providing a coherent set of requirements and recommendations to achieve interoperability. The pillars of the framework are the following technical documents[^9]:

-   The *Definition of Annex Themes and Scope* describes in greater detail the spatial data themes defined in the Directive, and thus provides a sound starting point for the thematic aspects of the data specification development.

-   The *Generic Conceptual Model* defines the elements necessary for interoperability and data harmonisation including cross-theme issues. It specifies requirements and recommendations with regard to data specification elements of common use, like the spatial and temporal schema, unique identifier management, object referencing, some common code lists, etc. Those requirements of the Generic Conceptual Model that are directly implementable are included in the Implementing Rule on Interoperability of Spatial Data Sets and Services.

-   The *Methodology for the Development of Data Specifications* defines a repeatable methodology. It describes how to arrive from user requirements to a data specification through a number of steps including use-case development, initial specification development and analysis of analogies and gaps for further specification refinement.

-   The *Guidelines for the Encoding of Spatial Data* defines how geographic information can be encoded to enable transfer processes between the systems of the data providers in the Member States. Even though it does not specify a mandatory encoding rule it sets GML (ISO 19136) as the default encoding for INSPIRE.

-   The *Guidelines for the use of Observations & Measurements and Sensor Web Enablement-related standards in INSPIRE Annex II and III data specification development* provides guidelines on how the "Observations and Measurements" standard (ISO 19156) is to be used within INSPIRE.

-   The *Common data models* are a set of documents that specify data models that are referenced by a number of different data specifications. These documents include generic data models for networks, coverages and activity complexes.

The structure of the data specifications is based on the "ISO 19131 Geographic information - Data product specifications" standard. They include the technical documentation of the application schema, the spatial object types with their properties, and other specifics of the spatial data themes using natural language as well as a formal conceptual schema language[^10].

A consolidated model repository, feature concept dictionary, and glossary are being maintained to support the consistent specification development and potential further reuse of specification elements. The consolidated model consists of the harmonised models of the relevant standards from the ISO 19100 series, the INSPIRE Generic Conceptual Model, and the application schemas[^11] developed for each spatial data theme. The multilingual INSPIRE Feature Concept Dictionary contains the definition and description of the INSPIRE themes together with the definition of the spatial object types present in the specification. The INSPIRE Glossary defines all the terms (beyond the spatial object types) necessary for understanding the INSPIRE documentation including the terminology of other components (metadata, network services, data sharing, and monitoring).

By listing a number of requirements and making the necessary recommendations, the data specifications enable full system interoperability across the Member States, within the scope of the application areas targeted by the Directive. The data specifications (in their version 3.0) are published as technical guidelines and provide the basis for the content of the Implementing Rule on Interoperability of Spatial Data Sets and Services[^12]. The content of the Implementing Rule is extracted from the data specifications, considering short- and medium-term feasibility as well as cost-benefit considerations. The requirements included in the Implementing Rule are legally binding for the Member States according to the timeline specified in the INSPIRE Directive.

In addition to providing a basis for the interoperability of spatial data in INSPIRE, the data specification development framework and the thematic data specifications can be reused in other environments at local, regional, national and global level contributing to improvements in the coherence and interoperability of data in spatial data infrastructures.

**Coordinate Reference Systems -- Executive Summary**

*Coordinate reference systems* are included in Annex I, which means that they are considered as reference data, i.e. data that constitute the spatial frame for linking and/or pointing to other information that belong to specific thematic fields as defined in the INSPIRE Annexes II and III.

The INSPIRE specification on *Coordinate reference systems* has been prepared following the participative principle of a consensus building process. The stakeholders, based on their registration as a Spatial Data Interest Community (SDIC) or a Legally Mandated Organisation (LMO) had the opportunity to bring forward user requirements and reference materials, propose experts for the specification development, and participate in the review of the data specifications. The Thematic Working Group responsible for the specification development was composed of geodetic and mapping experts coming from Portugal, Slovenia, France, Germany, Italy, Sweden, the UK and the Netherlands, all of them for many years involved in activities aiming to establish uniform geo-referencing within Europe. Due to the close links between and the special technical nature of the two themes of C*oordinate reference systems* and *Geographical grid systems*, the specifications of both themes were developed by one thematic working group.

*Coordinate reference systems* (hereafter: CRS) play a specific role that is quite different from the other themes in the Directive's annexes. Contrary to the other themes the *CRS* specification does [not]{.ul} concern a downloadable or viewable thematic data set. Rather, it presents a basic functionality allowing the harmonised and interoperable geographic localisation of spatial objects defined by the other INSPIRE thematic data specifications. Therefore, the methodology developed by the Drafting Team Data Specifications is only partly applicable to the work of this Thematic Working Group.

The specific task of the definition of the CRS therefore consists in taking the right decisions on the choice of one (or a limited number of) coordinate reference systems and map projections that will ensure a common basis for the geographical harmonisation between all the other themes defined in the Annexes of the Directive. There are however themes for which in addition to linear systems (that are usually used for the horizontal component) parametric, or on non-length-based systems[^13] are used for the vertical component.

This document provides the result of the specification of the CRS. It contains elements that form part of the Implementing Rule on Interoperability of Spatial Data Sets and Services. These elements are clearly indicated in the document as "IR Requirements". The other parts of the documents give clarification, background information and examples and are intended as part of the technical guidance documents accompanying the Implementing Rule.

The cornerstone of the specification development was the definition of the Directive on *Coordinate reference systems* as being *"*Systems for uniquely referencing spatial information in space as a set of coordinates (X, Y, Z) and/or latitude and longitude and height, based on a geodetic horizontal and vertical datum".

For the three-dimensional and two-dimensional coordinate reference systems and the horizontal component of compound coordinate reference systems used for making available the INSPIRE spatial data sets available, the datum shall be the datum of the European Terrestrial Reference System 1989 (ETRS89) in areas within its geographical scope, or the datum of the International Terrestrial Reference System (ITRS) or other geodetic coordinate reference systems compliant with ITRS in areas that are outside the geographical scope of ETRS89. Compliant with the ITRS means that the system definition is based on the definition of the ITRS and there is a well documented relationship between both systems, according to EN ISO 19111:2007.

For the vertical component on land, the European Vertical Reference System (EVRS) shall be used to express gravity-related heights within its geographical scope. Other vertical reference systems related to the Earth gravity field shall be used to express gravity-related heights in areas that are outside the geographical scope of EVRS.

Taking into account the outcomes regarding parametric reference systems for the vertical component in the free atmosphere, barometric pressure, converted to height using ISO 2533:1975 International Standard Atmosphere, or other linear or parametric reference systems shall be used. Where other parametric reference systems are used, these shall be described in an accessible reference using EN ISO 19111-2:2012.

The coordinate reference systems for the expression of the vertical component in marine areas has been refined by the Elevation thematic working group of the INSPIRE annex II theme. For depth values of the sea floor in marine areas with an appreciable tidal range, depths shall be referenced to the Lowest Astronomical Tide (LAT), as has already been mandated by Technical Resolution A2.5 of the International Hydrographic Organisation (IHO). In marine areas without an appreciable tidal range, in open oceans and effectively in waters deeper than 200 metres (where tide is not measured, since it has no significant impact on the accuracy of the sounding), the Mean Sea Level (MSL) or a well-defined reference level close to the MSL shall be used as the reference surface.

The referencing by parameters and temporal reference systems is out of the scope of the theme CRS. However, when data is exchanged using such reference systems, these shall be described in an accessible reference using EN ISO 19111-2:2012 or linked by reference.

The requirements and recommendations related to Map projections are based on the results from the "Map Projections for Europe" workshop[^14]. These are:

-   Lambert Azimuthal Equal Area (ETRS89-LAEA) for pan-European spatial analysis and reporting, where true area representation is required;

-   Lambert Conformal Conic (ETRS89-LCC) for conformal pan-European mapping at scales smaller than or equal to 1:500,000;

-   Transverse Mercator (ETRS89-TMzn) for conformal pan-European mapping at scales larger than 1:500,000.

These projections shall be available in INSPIRE transformation services.

For regions outside of continental Europe, for example for overseas MS territories, the MS shall define a map projection they consider most suitable for the purpose. Moreover, different INSPIRE themes or applications may use appropriate map projections, for example if the data characteristics require large scale mapping. In these cases the map projections shall be well documented to allow the conversion to geographic coordinates and an identifier shall be created, according to ISO 19111:2007.

For the rendering of spatial information for INSPIRE View Services, and in case there is a need for plane coordinates, the "Plate-Carrée" projection is recommended for the non-polar regions. For the polar regions a Polar stereographic projection is recommended. However, for the display of spatial data sets in such services at least the coordinate reference systems for two-dimensional geodetic coordinates (latitude, longitude) shall be available. This way, if data is stored in geographic coordinates there is no need for re-projecting.

This document contains also the identifiers for the different types of coordinate reference systems that shall be used.

**Acknowledgements**

Many individuals and organisations have contributed to the development of these Guidelines.

The Thematic Working Group Coordinate Reference Systems (TWG-RS) included:

João Torres (TWG Facilitator), Vida Bitenc (TWG Editor), Alessandro Caporali, Paul Crudace, Lars Engberg, Bruno Garayt, Heinz Habrich (regular members), Gil Ross Leendert Dorst, Jordi Escriu (external experts). Freddy Fierens (European Commission contact point).

Other contributors to the INSPIRE data specifications are the Drafting Team Data Specifications, the JRC Data Specifications Team and the INSPIRE stakeholders - Spatial Data Interested Communities (SDICs) and Legally Mandated Organisations (LMOs).

**Contact information**

Maria Vanda Nunes de Lima & Michael Lutz

European Commission Joint Research Centre (JRC)

Institute for Environment and Sustainability

Unit H06: Digital Earth and Reference Data

*http://inspire.ec.europa.eu/index.cfm/pageid/2*

**\
Table of contents**

::: {custom-style="toc 1"}
[1]{custom-style="Hyperlink"} [Scope]{custom-style="Hyperlink"} **Error! Bookmark not defined.**
:::

::: {custom-style="toc 1"}
[2]{custom-style="Hyperlink"} [Overview]{custom-style="Hyperlink"} 1
:::

::: {custom-style="toc 2"}
[2.1]{custom-style="Hyperlink"} [Name]{custom-style="Hyperlink"} 1
:::

::: {custom-style="toc 2"}
[2.2]{custom-style="Hyperlink"} [Informal description]{custom-style="Hyperlink"} 1
:::

::: {custom-style="toc 2"}
[2.3]{custom-style="Hyperlink"} [Normative References]{custom-style="Hyperlink"} 2
:::

::: {custom-style="toc 2"}
[2.4]{custom-style="Hyperlink"} [Terms and definitions]{custom-style="Hyperlink"} 3
:::

::: {custom-style="toc 2"}
[2.5]{custom-style="Hyperlink"} [Symbols and abbreviations]{custom-style="Hyperlink"} 3
:::

::: {custom-style="toc 2"}
[2.6]{custom-style="Hyperlink"} [How the Technical Guidelines map to the Implementing Rules]{custom-style="Hyperlink"} **Error! Bookmark not defined.**
:::

::: {custom-style="toc 3"}
[2.6.1]{custom-style="Hyperlink"} [Requirements]{custom-style="Hyperlink"} **Error! Bookmark not defined.**
:::

::: {custom-style="toc 3"}
[2.6.2]{custom-style="Hyperlink"} [Recommendations]{custom-style="Hyperlink"} **Error! Bookmark not defined.**
:::

::: {custom-style="toc 3"}
[2.6.3]{custom-style="Hyperlink"} [Conformance]{custom-style="Hyperlink"} **Error! Bookmark not defined.**
:::

::: {custom-style="toc 1"}
[3]{custom-style="Hyperlink"} [Specification scopes]{custom-style="Hyperlink"} 6
:::

::: {custom-style="toc 1"}
[4]{custom-style="Hyperlink"} [Identification information]{custom-style="Hyperlink"} **Error! Bookmark not defined.**
:::

::: {custom-style="toc 1"}
[5]{custom-style="Hyperlink"} [Coordinate Reference Systems]{custom-style="Hyperlink"} 7
:::

::: {custom-style="toc 2"}
[5.1]{custom-style="Hyperlink"} [Overview]{custom-style="Hyperlink"} 7
:::

::: {custom-style="toc 2"}
[5.2]{custom-style="Hyperlink"} [General description]{custom-style="Hyperlink"} 7
:::

::: {custom-style="toc 2"}
[5.3]{custom-style="Hyperlink"} [Datums for three-dimensional and two-dimensional coordinate reference systems]{custom-style="Hyperlink"} 8
:::

::: {custom-style="toc 3"}
[5.3.1]{custom-style="Hyperlink"} [Geodetic reference systems]{custom-style="Hyperlink"} 8
:::

::: {custom-style="toc 2"}
[5.4]{custom-style="Hyperlink"} [Coordinate reference systems]{custom-style="Hyperlink"} 9
:::

::: {custom-style="toc 3"}
[5.4.1]{custom-style="Hyperlink"} [Three-dimensional coordinate reference systems]{custom-style="Hyperlink"} 9
:::

::: {custom-style="toc 3"}
[5.4.2]{custom-style="Hyperlink"} [Two-dimensional coordinate reference systems]{custom-style="Hyperlink"} 9
:::

::: {custom-style="toc 3"}
[5.4.3]{custom-style="Hyperlink"} [Compound coordinate reference systems]{custom-style="Hyperlink"} 12
:::

::: {custom-style="toc 3"}
[5.4.4]{custom-style="Hyperlink"} [Other coordinate reference systems]{custom-style="Hyperlink"} 14
:::

::: {custom-style="toc 2"}
[5.5]{custom-style="Hyperlink"} [Identifiers]{custom-style="Hyperlink"} 15
:::

::: {custom-style="toc 1"}
[Bibliography]{custom-style="Hyperlink"} 17
:::

::: {custom-style="toc 1"}
[Annex A (normative) Abstract Test Suite]{custom-style="Hyperlink"} 19
:::

# 

# Scope

This document specifies a harmonised data specification for the spatial data theme *Coordinate Reference Systems* as defined in Annex I of the INSPIRE Directive.

This data specification provides the basis for the drafting of Implementing Rules according to Article 7 (1) of the INSPIRE Directive \[Directive 2007/2/EC\]. The entire data specification is published as implementation guidelines accompanying these Implementing Rules.

# Overview

## Name

INSPIRE data specification for the theme Coordinate Reference Systems.

## Informal description

**[Definition:]{.ul}**

Systems for uniquely referencing spatial information in space as a set of coordinates (X, Y, Z) and/or latitude, longitude and height, based on a geodetic horizontal and vertical datum.

\[Directive 2007/2/EC\]

**[Description:]{.ul}**

The scope of the theme *Coordinate reference systems* covers the Geodetic Coordinate Reference Systems (CRS) required for uniquely referencing spatial information in space as a set of coordinates (X, Y, Z) and/or latitude (φ), longitude (λ) and either ellipsoidal (h) or gravity-related height (H).

This specification establishes:

a.  The geodetic datums and coordinate reference systems to be used when making spatial data sets available for INSPIRE, unless otherwise required for data of a specific theme.

> Particularly, the following ones are adopted:

-   The European Terrestrial Reference System 1989 (ETRS89), as geodetic datum within its scope.

-   The European Vertical Reference System (EVRS), to express gravity-related heights on land within its scope.

-   Barometric pressure, converted to height using ISO 2533:1975 International Standard Atmosphere, to express heights in the free atmosphere.

-   The Lowest Astronomical Tide (LAT), as reference surface to express depth values representing the sea floor in marine areas with an appreciable tidal range.

-   The Mean Sea Level (MSL), or a well-defined reference level close to the MSL, as reference surface to express depth values representing the sea floor in marine areas without an appreciable tidal range, in open oceans and effectively in waters deeper than 200 metres.

b.  Plane coordinates reference systems (map projections) adopted and recommended for different purposes, covering the requirements of the INSPIRE transformation services and view services as well.

> Particularly, at least the coordinate reference systems for two-dimensional geodetic coordinates (latitude, longitude) shall be available for the display of spatial data sets with the view network service (Regulation No 976/2009[^15]).

c.  The identifiers for the different types of coordinates that shall be used.

The document also provides rules and guidance on geodetic coordinate reference systems, vertical reference systems and map projections for their use outside of continental Europe (e.g. overseas territories).

In general the referencing by parameters and temporal reference systems are out of scope of the theme CRS.

## Normative References

\[Directive 2007/2/EC\] Directive 2007/2/EC of the European Parliament and of the Council of 14 March 2007 establishing an Infrastructure for Spatial Information in the European Community (INSPIRE)

\[IHO TRA2.5\] Datums and Benchmarks in IHO M3 Resolutions of the International Hydrographic Organization, version updated to September 2008

\[IHO S32\] Hydrographic Dictionary, 5th edition, 1994

\[IHO S44\] Standards for Hydrographic Surveys, 5th edition, February 2008

\[ISO 2533\] ISO 2533:1975, International Standard Atmosphere

\[ISO 6709\] ISO 6709:2008 (Standard representation of geographical point position by coordinates)

\[ISO 19111\] EN ISO 19111:2007 Geographic information - Spatial referencing by coordinates (ISO 19111:2007)

\[ISO 19111-2\] EN ISO 19111-2:2012 Geographic information - Spatial referencing by coordinates -- Part 2: Extension for parametric values

\[ISO 19115\] EN ISO 19115:2005, Geographic information -- Metadata (ISO 19115:2003)

\[ISO/TS 19127\] ISO/TS 19127:2005, Geographic information \-- Geodetic codes and parameters

\[ISO 19135\] EN ISO 19135:2007 Geographic information -- Procedures for item registration (ISO 19135:2005)

\[Regulation 1205/2008/EC\] Regulation 1205/2008/EC implementing Directive 2007/2/EC of the European Parliament and of the Council as regards metadata

## Terms and definitions

General terms and definitions helpful for understanding the INSPIRE data specification documents are defined in the INSPIRE Glossary[^16].

Specifically, for the theme Coordinate Reference Systems, the following terms are defined:

**(1) compound coordinate reference system**

Coordinate reference system using two independent coordinate reference systems, one for the horizontal component and one for the vertical component, to describe a position \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

**(2) coordinate reference system**

Coordinate system which is related to the real world by a datum \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

NOTE This definition includes coordinate systems based on geodetic or cartesian coordinates and coordinate systems based on map projections.

**(3) coordinate system**

Set of mathematical rules for specifying how coordinates are to be assigned to points \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

**(4) datum**

Parameter or set of parameters that define the position of the origin, the scale, and the orientation of a coordinate system \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

**(5) geodetic coordinate system**

Coordinate system in which position is specified by geodetic latitude, geodetic longitude and (in the three-dimensional case) ellipsoidal height \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

**(6) geodetic datum**

Datum describing the relationship of a coordinate system to the Earth \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

**(7) lowest astronomical tide**

(LAT) Lowest tide level which can be predicted to occur under average meteorological conditions and under any combination of astronomical conditions \[IHO TRA2.5\]

**(8) map projection**

Change of coordinates, based on a one-to-one relationship, from a geodetic coordinate system to a plane, based on the same datum \[EN ISO 19111:2007, Geographic information --- Spatial referencing by coordinates\]

**(9) mean sea level**

(MSL) Average height of the surface of the sea at a tide station for all stages of the tide over a 19-year period, usually determined from hourly height readings measured from a fixed predetermined reference level (chart datum) \[IHO TRA2.5\]

## Symbols and abbreviations

CRS Coordinate Reference System

EC European Commission

ETRS89 European Terrestrial Reference System 1989

ETRS89-EVRS Compound Coordinate Reference System ETRS89-EVRS

ETRS89-LAEA Projection Lambert Azimuthal Equal Area

ETRS89-LCC Projection Lambert Conformal Conic

ETRS89-TMzn Projection Transverse Mercator

EUREF Reference Frame Sub-commission for Europe of the IAG

EVRS European Vertical Reference System

GCM Generic Conceptual Model

GRS80 Geodetic Reference System 1980

IAG International Association of Geodesy

ICAO International Civil Aviation Organisation

IERS International Earth Rotation and Reference Systems Service

IHO International Hydrographic Organisation

ISA International Standard Atmosphere

ITRF International Terrestrial Reference Frame

ITRS International Terrestrial Reference System

IUGG International Union of Geodesy and Geophysics

JRC Joint Research Centre

LAT Lowest Astronomical Tide

MS Member States

MSL Mean Sea Level

TRS Terrestrial Reference System

TWG Thematic Working Group

VRF Visual Flying Rules

## How the Technical Guidelines map to the Implementing Rules

The schematic diagram in Figure 1 gives an overview of the relationships between the INSPIRE legal acts (the INSPIRE Directive and Implementing Rules) and the INSPIRE Technical Guidelines. The INSPIRE Directive and Implementing Rules include legally binding requirements that describe, usually on an abstract level, *what* Member States must implement.

In contrast, the Technical Guidelines define *how* Member States might implement the requirements included in the INSPIRE Implementing Rules. As such, they may include non-binding technical requirements that must be satisfied if a Member State data provider chooses to conform to the Technical Guidelines. Implementing these Technical Guidelines will maximise the interoperability of INSPIRE spatial data sets.

![](media/image4.png){width="6.2875in" height="3.90625in"}

::: {custom-style="caption"}
Figure 1 - Relationship between INSPIRE Implementing Rules and Technical Guidelines
:::

### Requirements

The purpose of these Technical Guidelines (Data specifications on *Coordinate Reference Systems*) is to provide practical guidance for implementation that is guided by, and satisfies, the (legally binding) requirements included for the spatial data theme Coordinate Reference Systems in the Regulation (Implementing Rules) on interoperability of spatial data sets and services. These requirements are highlighted in this document as follows:

> **IR Requirement**
>
> *Article / Annex / Section no.*
>
> **Title / Heading**
>
> This style is used for requirements contained in the Implementing Rules on interoperability of spatial data sets and services (Commission Regulation (EU) No 1089/2010).

::: {custom-style="header"}
For each of these IR requirements, these Technical Guidelines contain additional explanations and examples.
:::

::: {custom-style="header"}
NOTE The Abstract Test Suite (ATS) in Annex A contains conformance tests that directly check conformance with these IR requirements.
:::

::: {custom-style="header"}
Furthermore, these Technical Guidelines may propose a specific technical implementation for satisfying an IR requirement. In such cases, these Technical Guidelines may contain additional technical requirements that need to be met in order to be conformant with the corresponding IR requirement *when using this proposed implementation*. These technical requirements are highlighted as follows:
:::

> **TG Requirement X** This style is used for requirements for a specific technical solution proposed in these Technical Guidelines for an IR requirement.

::: {custom-style="header"}
NOTE 1 Conformance of a data set with the TG requirement(s) included in the ATS implies conformance with the corresponding IR requirement(s).
:::

NOTE 2 In addition to the requirements included in the Implementing Rules on interoperability of spatial data sets and services, the INSPIRE Directive includes further legally binding obligations that put additional requirements on data providers. For example, Art. 10(2) requires that Member States shall, where appropriate, decide by mutual consent on the depiction and position of geographical features whose location spans the frontier between two or more Member States. General guidance for how to meet these obligations is provided in the INSPIRE framework documents.

### Recommendations

::: {custom-style="header"}
In addition to IR and TG requirements, these Technical Guidelines may also include a number of recommendations for facilitating implementation or for further and coherent development of an interoperable infrastructure.
:::

> **Recommendation X** Recommendations are shown using this style.

NOTE The implementation of recommendations is not mandatory. Compliance with these Technical Guidelines or the legal obligation does not depend on the fulfilment of the recommendations.

### Conformance

Annex A includes the abstract test suite for checking conformance with the requirements included in these Technical Guidelines and the corresponding parts of the Implementing Rules (Commission Regulation (EU) No 1089/2010).

# Specification scopes

This data specification does not distinguish different specification scopes, but just considers one general scope.

NOTE For more information on specification scopes, see \[ISO 19131:2007\], clause 8 and Annex D.

::: {custom-style="annotation text"}
:::

# Identification information

These Technical Guidelines are identified by the following URI:

http://inspire.ec.europa.eu/tg/rs/3.2

NOTE ISO 19131 suggests further identification information to be included in this section, e.g. the title, abstract or spatial representation type. The proposed items are already described in the document metadata, executive summary, overview description (section 2) and descriptions of the application schemas (section 5). In order to avoid redundancy, they are not repeated here.

# Coordinate Reference Systems {#coordinate-reference-systems .head1}

## Overview

The INSPIRE theme *Coordinate reference systems* (CRS) provides a harmonised specification for uniquely referencing spatial information, either using three-dimensional, two-dimensional or compound coordinate reference systems for determining the horizontal and vertical components.

This document also provides the specification for the map projections to be used for geo-referencing the spatial information in plane coordinates.

The mandated CRS can be used for any kind of information/resolution/accuracy; the resolution and accuracy of data are out of scope of the theme CRS.

For data sets with low positional accuracy, the original CRS of the data set may sometimes be considered equivalent to the mandated CRS. It is recommended that the data set provider consults the experts in the Member States (MS) to evaluate the need to transform the data sets from the original CRS to the mandated CRS. The decision for the maintenance of the data sets in its original CRS or in the mandated CRS will be taken according to the MS and the INSPIRE regulations.

The accuracy of the data sets resulting from transformations and conversion formulas are out of scope of the theme CRS. The accuracy of the data sets must be documented by the data set provider according to all the aspects that contribute to it, namely the original data accuracy and the accuracy of the conversions, transformations and other aspects involved with the management of the data.

There are themes for which data are expressed in linear systems for the horizontal component or on non-length-based vertical systems like pressure, density, for the vertical component. This kind of referencing is parametric. In general the referencing by parameters is out of scope of the theme CRS. It is recommended to associate the parameters with the specific data according to EN ISO 19111-2 (Extension for parametric values).

Atmospheric and oceanographic communities use specific parametric reference systems for the expression of the vertical component. In the free ocean depths, observations of temperature, salinity etc. have no direct height measure. Pressure is the parametric reference system used and any measure of depth is an approximation or inferred value based on the vertical profile. In contrast, in the free atmosphere aircraft use barometric pressure, scaled as heights according to the International Standard Atmosphere (defined by ISO 2533:1975) and appropriately calibrated to a surface datum to ensure separation. Relative height differences measured by pressure are not appreciably affected by changes in the actual surface pressure (no direct height measurements are used). Therefore parametric references using barometric pressure converted to height are adopted for INSPIRE in this specification to express the vertical component in the free atmosphere. These reference systems has been refined by the respective INSPIRE TWGs of annex II and III themes.

Specifying systems with more general parametric elements is out of scope. Nevertheless when such systems are used it is recommended that they should be appropriately specified and referenced.

Finally, there are themes that may require temporal references. Such reference systems are also out of scope of the theme CRS.

## General description

Geodetic Coordinate Reference Systems (CRS) define the constants and parameters needed for geodetic datums, and are required for uniquely referencing spatial information in space as a set of coordinates (X, Y, Z) and/or latitude (φ), longitude (λ) and either ellipsoidal (h) or gravity-related height (H). The datums include horizontal datum for φ and λ and a vertical datum to express either ellipsoidal or gravity-related heights, to form a compound coordinate reference system.

The set of coordinates (φ, λ, h) can be derived from the space set of coordinates (X, Y, Z) using a suitable reference ellipsoid. The GRS80 ellipsoid is adopted for this purpose.

Plane coordinates may be derived from latitude and longitude using suitable cartographic projections.

## Datums for three-dimensional and two-dimensional coordinate reference systems

This section specifies the datums required for the provision of INSPIRE data using two-dimensional or three-dimensional CRS.

### Geodetic reference systems

The coordinate reference systems used in the majority of the European region are linked to the Eurasian tectonic plate. The European Terrestrial Reference System 1989 (ETRS89) is in principle tied to the stable part of this plate. Since Directive 2007/2/EC also affects areas that are not on the Eurasian tectonic plate, it is necessary that the rules concerning coordinate reference systems take also into account areas that are not considered to be on the Eurasian tectonic plate. This kind of situation occurs, for example, in the European countries\' overseas territories.

The International Terrestrial Reference System (ITRS) \[IERS\] is presently the recommended Terrestrial Reference System (TRS) for the whole geo-science community, through a resolution adopted by the International Union of Geodesy and Geophysics (IUGG) during its General Assembly of Perugia in 2007. The primary realisations of ITRS are created through an optimal combined use of space geodetic techniques; they are released to the international community and labelled International Terrestrial Reference Frames: (ITRFyy).

These primary realisations are also densified and disseminated through regional, national and local terrestrial geodetic networks. The European Terrestrial Reference System 1989 (ETRS89) \[EUREF\] is related to the ITRS and its realisations are designated by European Terrestrial Reference Frames: (ETRFyy).

The WGS84 system designates a full set of geodetic standards, in which successive realisations of a unique TRS has been provided. The most recent WGS84 realisations are in agreement with the ITRF at the level of a few centimetres. In consequence, the WGS84 products (as concerning TRS issues) are considered as realisations of the ITRS. The WGS84 is linked to the ITRS.

The MS have extended the ETRS89 to their continental and neighbour territories through their own realisations that are linked to the ETRFyy solutions. The European continental and neighbour territories of the MS constitute the geographical scope of the ETRS89.

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.2*
:::

::: {custom-style="IR requirement grey"}
**Datum for three-dimensional and two-dimensional coordinate reference systems**
:::

::: {custom-style="IR requirement grey"}
For the three-dimensional and two-dimensional coordinate reference systems and the horizontal component of compound coordinate reference systems used for making spatial data sets available, the datum shall be the datum of the European Terrestrial Reference System 1989 (ETRS89) in areas within its geographical scope, or the datum of the International Terrestrial Reference System (ITRS) or other geodetic coordinate reference systems compliant with ITRS in areas that are outside the geographical scope of ETRS89. Compliant with the ITRS means that the system definition is based on the definition of the ITRS and there is a well documented relationship between both systems, according to EN ISO 19111:2007.
:::

## Coordinate reference systems

This section specifies the different types of coordinate reference systems available for the provision of INSPIRE data at European level.

### Three-dimensional coordinate reference systems

Three-dimensional CRS are used to express both, the horizontal and the vertical components of geographical locations. This may be performed by means of:

-   Cartesian CRS, where X, Y, and Z coordinates are used to define the location, or;

-   Three-dimensional geodetic CRS, where latitude, longitude and ellipsoidal height define the location.

The following requirement establishes the three-dimensional CRS which are allowed in the INSPIRE context.

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.3*
:::

::: {custom-style="IR requirement grey"}
**Coordinate Reference Systems**
:::

::: {custom-style="IR requirement grey"}
Spatial data sets shall be made available using at least one of the coordinate reference systems specified in sections 1.3.1, 1.3.2 and 1.3.3, unless one of the conditions specified in section 1.3.4 holds.
:::

::: {custom-style="IR requirement grey"}
**1.3.1. Three-dimensional Coordinate Reference Systems**
:::

-   ::: {custom-style="IR requirement grey"}
    > Three-dimensional Cartesian coordinates based on a datum specified in 1.2 and using the parameters of the Geodetic Reference System 1980 (GRS80) ellipsoid.
    :::

-   ::: {custom-style="IR requirement grey"}
    > Three-dimensional geodetic coordinates (latitude, longitude and ellipsoidal height) based on a datum specified in 1.2 and using the parameters of the GRS80 ellipsoid.
    :::

    ::: {custom-style="IR requirement grey"}
    (...)
    :::

NOTE For the computation of latitude, longitude and ellipsoidal height, and for the computation of plane coordinates using a suitable mapping projection, it is proposed to use the parameters of the Geodetic Reference System 1980 (GRS80) ellipsoid (see below). The Geodetic Reference System 1980[^17] has been adopted at the XVII General Assembly of the IUGG in Canberra, December 1979.

### Two-dimensional coordinate reference systems

Two-dimensional CRS are used to express the horizontal component. This may be performed by means of:

-   Two-dimensional geodetic CRS, where latitude and longitude on a reference ellipsoid are used to define the horizontal location, or;

-   Plane CRS (suitable map projections), where a pair of coordinates - either (N, E) or (Y, X) - defines the horizontal location through the projection.

The following requirement establishes the two-dimensional CRS which are allowed in the INSPIRE context.

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.3*
:::

::: {custom-style="IR requirement grey"}
**Coordinate Reference Systems**
:::

::: {custom-style="IR requirement grey"}
Spatial data sets shall be made available using at least one of the coordinate reference systems specified in sections 1.3.1, 1.3.2 and 1.3.3, unless one of the conditions specified in section 1.3.4 holds.
:::

::: {custom-style="IR requirement grey"}
(...)
:::

::: {custom-style="IR requirement grey"}
**1.3.2. Two-dimensional Coordinate Reference Systems**
:::

-   ::: {custom-style="IR requirement grey"}
    > Two-dimensional geodetic coordinates (latitude and longitude) based on a datum specified in 1.2 and using the parameters of the GRS80 ellipsoid.
    :::

-   ::: {custom-style="IR requirement grey"}
    > Plane coordinates using the ETRS89 Lambert Azimuthal Equal Area coordinate reference system.
    :::

-   ::: {custom-style="IR requirement grey"}
    > Plane coordinates using the ETRS89 Lambert Conformal Conic coordinate reference system.
    :::

-   ::: {custom-style="IR requirement grey"}
    > Plane coordinates using the ETRS89 Transverse Mercator coordinate reference system.
    :::

    ::: {custom-style="IR requirement grey"}
    (...)
    :::

#### Map projections

Map projections are used for geo-referencing spatial information in plane coordinates.

Map projections are required to make possible the data delivery and exchange in this type of coordinates at the Pan-European level.

Between 14-15 December 2000 the "Map Projections for Europe" workshop^14^ was organised to propose the map projections to be used for representation of data in plane coordinates in general applications. The use of the following projections was recommended:

-   Lambert Azimuthal Equal Area (ETRS89-LAEA) for spatial analysis and display;

-   Lambert Conformal Conic (ETRS89-LCC) for conformal pan-European mapping at scales smaller or equal to 1:500,000;

-   Transverse Mercator (ETRS89-TMzn) for conformal pan-European mapping at scales larger than 1:500,000.

These recommendations have been used by the European Commission (EC) for geo-referencing the data internally within the EC. For the representation of data in plane coordinates in general pan-European applications in continental Europe in the frame of INSPIRE, these projections are either mandated or recommended. For regions outside of continental Europe, for example for overseas MS territories, the MS shall define a map projection they consider most suitable for the application. The ETRS89-LAEA projection in INSPIRE is recommended for spatial analysis and reporting.

The formulas of the above mentioned map projections are published in the proceedings of the "Map Projections for Europe" workshop (Marne-La Vallee, 14-15 December 2000) and in the proceedings of the "European Reference Grids" workshop (Ispra, 27-29 October 2003). For other map projections, see Snyder, John P: Map Projections -- A Working Manual (Snyder, 1987).

The Transverse Mercator (ETRS89-TMzn) is identical to the Universal Transverse Mercator (UTM) grid system for the Northern hemisphere when applied to the ETRS89 geodetic datum and the GRS80 ellipsoid. The UTM system was developed for worldwide application between 80º S and 84º N.

1.  ::: {custom-style="Recommendation"}
    > For pan-European spatial analysis and reporting, where true area representation is required, the ETRS89-LAEA is recommended
    :::

2.  ::: {custom-style="Recommendation"}
    > For conformal pan-European mapping at scales smaller than or equal to 1:500,000, the ETRS89-LCC is recommended
    :::

3.  ::: {custom-style="Recommendation"}
    > For conformal pan-European mapping at scales larger than 1:500,000, the Transverse Mercator ETRS89-TMzn is recommended
    :::

4.  ::: {custom-style="Recommendation"}
    > It is recommended that the projections referred in section 1.3.2 of Annex II of Commission Regulation (EU) No 1089/2010) are available in INSPIRE transformation services.
    :::

Users may benefit of INSPIRE download and transformation services to get and re-project datasets according their aims. Moreover, different INSPIRE themes or applications where INSPIRE compliant data is integrated should use appropriate map projections. This is especially important when analysis is being done in large scales.

#### Coordinate Reference Systems used in the View Network Service 

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.4*
:::

::: {custom-style="IR requirement grey"}
**Coordinate Reference Systems used in the View Network Service**
:::

::: {custom-style="IR requirement grey"}
For the display of spatial data sets with the view network service as specified in Regulation No 976/2009[^18], at least the coordinate reference systems for two-dimensional geodetic coordinates (latitude, longitude) shall be available.
:::

::: {custom-style="annotation text"}
To show geodetic coordinates on a planar two-dimensional map for the view service or other purposes, they need to be projected. For the relevant requirements and recommendations on the appropriate projection to be used please consult the View Service Technical Guidelines \[ViewServiceTG\].
:::

::: {custom-style="annotation text"}
NOTE As stated in section 7.3.5 of ISO 19128:2005 \[ISO 19128\] (WMS 1.3.0): "when the CRS parameter specifies a geographic coordinate reference system (...), the spatial data is internally projected using the Pseudo Plate Carrée coordinate operation method and thereafter transformed to an image coordinate reference system with the *i* axis parallel and proportional to longitude and the *j* axis parallel and proportional to latitude to enable direct screen rendering."
:::

::: {custom-style="annotation text"}
The Plate-Carrée projection is one of the most simple and intuitive map projections for rendering spatial information on a two-dimensional map. It is a specific case of the equirectangular projection (also called equidistant cylindrical projection), which obtains a symmetric graticule by transforming meridians to vertical equally-spaced straight parallel lines half as long as the Equator, and parallels to horizontal equally-spaced straight lines perpendicular to and having the same spacing as meridians. The Poles become straight lines equal in length to the Equator.
:::

::: {custom-style="annotation text"}
The projection is neither equal area nor conformal because of the distortions it introduces, having little use in navigation or cadastral mapping. However it is often used in thematic mapping of regional areas or of the whole world. In particular, the Plate Carrée has become a de facto standard for global raster datasets because of the particularly simple relationship between the position of an image pixel on the map and its corresponding geographic location on Earth.
:::

::: {custom-style="annotation text"}
For the display of spatial information on the screen the most important features are the ability of the application to give the pixel coordinates true projected coordinates and to facilitate the overlaying of different sources of spatial information, while taking into account the economic aspects of putting online spatial information from the Member States. The cost of using the equirectangular Plate Carrée for projecting is lower than other methods available, such as the Mercator cylindrical spherical projection.
:::

### Compound coordinate reference systems

A compound CRS is a coordinate reference system that combines a two-dimensional CRS (the horizontal component) with a one-dimensional CRS (the vertical component). It allows unambiguous 3D geo-referencing.

EXAMPLE Geodetic coordinates in ETRS89 using the GRS80 ellipsoid combined with heights in EVRS form a compound CRS

For the horizontal component, any of the two-dimensional CRS specified in section 5.4.2 may be used.

This section lists the one-dimensional CRS that may be used as the vertical datum to express the vertical component (heights or depths) of compound reference systems. Different vertical reference systems are proposed for land areas, the free atmosphere and marine areas. These are explained in more detail in the following sub-sections.

The following requirement specifies the allowed combinations of coordinate reference systems for the horizontal and the vertical components.

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.3*
:::

::: {custom-style="IR requirement grey"}
**Coordinate Reference Systems**
:::

::: {custom-style="IR requirement grey"}
Spatial data sets shall be made available using at least one of the coordinate reference systems specified in sections 1.3.1, 1.3.2 and 1.3.3, unless one of the conditions specified in section 1.3.4 holds.
:::

::: {custom-style="IR requirement grey"}
(...)
:::

::: {custom-style="IR requirement grey"}
**1.3.3. Compound Coordinate Reference Systems**
:::

::: {custom-style="IR requirement grey"}
1\. For the horizontal component of the compound coordinate reference system, one of the coordinate reference systems specified in section 1.3.2 shall be used.
:::

::: {custom-style="IR requirement grey"}
2\. For the vertical component, one of the following coordinate reference systems shall be used:
:::

-   ::: {custom-style="IR requirement grey"}
    > For the vertical component on land, the European Vertical Reference System (EVRS) shall be used to express gravity-related heights within its geographical scope. Other vertical reference systems related to the Earth gravity field shall be used to express gravity-related heights in areas that are outside the geographical scope of EVRS.
    :::

-   ::: {custom-style="IR requirement grey"}
    > For the vertical component in the free atmosphere, barometric pressure, converted to height using ISO 2533:1975 International Standard Atmosphere, or other linear or parametric reference systems shall be used. Where other parametric reference systems are used, these shall be described in an accessible reference using EN ISO 19111-2:2012.
    :::

-   ::: {custom-style="IR requirement grey"}
    > For the vertical component in marine areas where there is an appreciable tidal range (tidal waters), the Lowest Astronomical Tide (LAT) shall be used as the reference surface.
    :::

-   ::: {custom-style="IR requirement grey"}
    > For the vertical component in marine areas without an appreciable tidal range, in open oceans and effectively in waters that are deeper than 200 meters, the Mean Sea Level (MSL) or a well-defined reference level close to the MSL shall be used as the reference surface.
    :::

    ::: {custom-style="IR requirement grey"}
    (...)
    :::

#### Land areas

The European Vertical Reference System (EVRS) \[EUREF\] is the vertical reference system to be used for Europe on land to express gravity-related heights. The most recent realisation of the EVRS is labelled European Vertical Reference Frame 2007 (EVRF2007). The definition of EVRS is described in the EVRS Conventions 2007.

The vertical reference systems for land existing in the MS can be expressed in the EVRS in their continental territories through their own realisations that are linked to the EVRF2007 solution. Future solutions of the EVRF will constitute an improvement and are considered realisations of the EVRS. The European continental territories of the MS constitute the geographical scope of the EVRS.

It is necessary that Member States define the vertical datum to be used outside European continental territories (see section 5.4.4), since they cannot be connected to the European vertical datum. In this case, a locally or globally defined vertical reference system related to the Earth gravity field will be used to express gravity-related heights.

#### Free atmosphere

In the free atmosphere, aircraft use barometric pressure, scaled as heights and appropriately calibrated to a surface datum to ensure separation. Atmospheric observations and measurements from aircraft therefore have the vertical coordinate measured as a barometric pressure.

Barometric pressure decreases monotonically with height, and to measure the exact height the full temperature profile in the vertical below the measurement must be known. This is seldom available directly, and indirect measurement of height requires estimation of this profile using numerical atmospheric models. At sufficiently elevated levels, an approximate conversion to height is used[^19].

The International Standard Atmosphere (ISA) \[ISO 2533\] is used for such purpose. It is calibrated in both, thousands of feet and metres (kilofeet is used in aviation, by law). It measures approximate geopotential height because the datum ignores the variation of the atmospheric temperature and pressure near the bottom of the atmosphere. Heights are named as flight levels (e.g. FL320 is nominally 32 thousand feet). Even if a true height measure is available in an aircraft (e.g. through radar or GPS) the readings must be converted to ISA flight levels -- unless the pilot is flying under Visual Flying Rules (VFR) near the ground. The origin of heights corresponds to the mean sea level pressure in the standard atmosphere: 1013.25 hPa (hectopascal).

However, other linear or parametric reference systems rather than ISO 2533:1975 International Standard Atmosphere may be used. In this case, these shall be appropriately described in an accessible reference using EN ISO 19111-2:2012.

#### Marine areas

For the free ocean, the profile in the deep ocean is typically measured by sounding buoys. These use pressure as a vertical measure and the datum is the actual ocean surface. When these buoys surface and transmit the measurements, the depths are usually supplied already converted by a calibration mechanism which also includes corrections for the temperature and salinity profiles, and for the compression effects of water under high pressure.

Otherwise depths are estimated using a hydrostatic approximation. For anything other than ocean modelling this is likely to be sufficient. Divers, submarines and tethered buoys only operate at shallow depths compared to deep oceans where the approximations become unacceptable.

The specification of the ocean surface datum has problems too. Although there are projects to use satellite measurements of the oceanic geoid, these are not universally available or used. Ocean modellers also have to consider diurnal variations in temperature in the immediate ocean surface.

For depth values of the sea floor in marine areas with an appreciable tidal range, depths are usually referenced to the Lowest Astronomical Tide (LAT), as has already been mandated by Technical Resolution A2.5 of the International Hydrographic Organisation (IHO). In marine areas without an appreciable tidal range, in open oceans and effectively in waters deeper than 200m, tide is not measured since it has no significant impact on the accuracy of the sounding. Therefore the Mean Sea Level (MSL) or a well-defined reference level close to the MSL is used as reference surface.

### Other coordinate reference systems

The exceptions stated in the following requirement applies to three-dimensional, two-dimensional coordinate reference systems (including map projections), and compound reference systems.

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.3*
:::

::: {custom-style="IR requirement grey"}
**Coordinate Reference Systems**
:::

::: {custom-style="IR requirement grey"}
Spatial data sets shall be made available using at least one of the coordinate reference systems specified in sections 1.3.1, 1.3.2 and 1.3.3, unless one of the conditions specified in section 1.3.4 holds.
:::

::: {custom-style="IR requirement grey"}
(...)
:::

::: {custom-style="IR requirement grey"}
**1.3.4. Other Coordinate Reference Systems**
:::

::: {custom-style="IR requirement grey"}
Exceptions, where other coordinate reference systems than those listed in 1.3.1, 1.3.2 or 1.3.3 may be used, are:
:::

::: {custom-style="IR requirement grey"}
1\. Other coordinate reference systems may be specified for specific spatial data themes in this Annex.
:::

::: {custom-style="IR requirement grey"}
2\. For regions outside of continental Europe, Member States may define suitable coordinate reference systems.
:::

::: {custom-style="IR requirement grey"}
The geodetic codes and parameters needed to describe these coordinate reference systems and to allow conversion and transformation operations shall be documented and an identifier shall be created, according to EN ISO 19111:2007 and ISO/TS 19127:2005.
:::

In case other map projections are used, they must be well documented to allow the conversion to geographic coordinates and an identifier created. The documentation shall be provided according to EN ISO 19111:2007, which states how a projected coordinate reference system must be described.

Any specific map projection requirements applicable to a particular INSPIRE theme is specified in the corresponding technical guideline.

EXAMPLE 1 Map projections used in atmospheric and meteorological data may not be restricted to those used in European land areas. Typically a Polar stereographic projection is used for these purposes.

EXAMPLE 2 For navigation at sea, Mercator projections are used except in Polar regions.

## Identifiers

::: {custom-style="IR requirement grey"}
**IR Requirement**
:::

::: {custom-style="IR requirement grey"}
*Annex II, Section 1.5*
:::

::: {custom-style="IR requirement grey"}
**Coordinate Reference Systems Identifiers**
:::

::: {custom-style="IR requirement grey"}
1\. Coordinate reference system parameters and identifiers shall be managed in one or several common registers for coordinate reference systems.
:::

::: {custom-style="IR requirement grey"}
2\. Only identifiers contained in a common register shall be used for referring to the coordinate reference systems listed in this Section.
:::

These Technical Guidelines propose to use the http URIs provided by the Open Geospatial Consortium as coordinate reference system identifiers (see identifiers for the default CRSs below). These are based on and redirect to the definition in the EPSG Geodetic Parameter Registry (*http://www.epsg-registry.org/*).

1.  ::: {custom-style="TG Requirement grey"}
    The identifiers listed in Table 1 shall be used for referring to the coordinate reference systems used in a data set.
    :::

NOTE CRS identifiers may be used e.g. in:

-   data encoding,

-   data set and service metadata, and

-   requests to INSPIRE network services.

::: {custom-style="caption"}
Table 1 - http URIs for the default coordinate reference systems
:::

+--------------------------------------------------------------+-------------------+----------------------------------------------+
| **Coordinate reference system**                              | **Short name**    | **http URI identifier**                      |
+==============================================================+===================+==============================================+
| 3D Cartesian in ETRS89                                       | ETRS89-XYZ        | *http://www.opengis.net/def/crs/EPSG/0/4936* |
|                                                              |                   |                                              |
| (X,Y,Z)                                                      |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 3D geodetic in ETRS89 on GRS80                               | ETRS89-GRS80h     | *http://www.opengis.net/def/crs/EPSG/0/4937* |
|                                                              |                   |                                              |
| (Latitude, Longitude, Ellipsoidal height)                    |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D geodetic in ETRS89 on GRS80                               | ETRS89-GRS80      | *http://www.opengis.net/def/crs/EPSG/0/4258* |
|                                                              |                   |                                              |
| (Latitude, Longitude)                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D LAEA projection in ETRS89                                 | ETRS89-LAEA       | *http://www.opengis.net/def/crs/EPSG/0/3035* |
|                                                              |                   |                                              |
| on GRS80                                                     |                   |                                              |
|                                                              |                   |                                              |
| (Y,X)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D LCC projection in ETRS89 on GRS80                         | ETRS89-LCC        | *http://www.opengis.net/def/crs/EPSG/0/3034* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 26N (30°W to 24°W) | ETRS89-TM26N      | *http://www.opengis.net/def/crs/EPSG/0/3038* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 27N (24°W to 18°W) | ETRS89-TM27N      | *http://www.opengis.net/def/crs/EPSG/0/3039* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 28N (18°W to 12°W) | ETRS89-TM28N      | *http://www.opengis.net/def/crs/EPSG/0/3040* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 29N (12°W to 6°W)  | ETRS89-TM29N      | *http://www.opengis.net/def/crs/EPSG/0/3041* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 30N (6°W to 0°)    | ETRS89-TM30N      | *http://www.opengis.net/def/crs/EPSG/0/3042* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 31N (0° to 6°E)    | ETRS89-TM31N      | *http://www.opengis.net/def/crs/EPSG/0/3043* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 32N (6°E to 12°E)  | ETRS89-TM32N      | *http://www.opengis.net/def/crs/EPSG/0/3044* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 33N (12°E to 18°E) | ETRS89-TM33N      | *http://www.opengis.net/def/crs/EPSG/0/3045* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 34N (18°E to 24°E) | ETRS89-TM34N      | *http://www.opengis.net/def/crs/EPSG/0/3046* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 35N (24°E to 30°E) | ETRS89-TM35N      | *http://www.opengis.net/def/crs/EPSG/0/3047* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 36N (30°E to 36°E) | ETRS89-TM36N      | *http://www.opengis.net/def/crs/EPSG/0/3048* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 37N (36°E to 42°E) | ETRS89-TM37N      | *http://www.opengis.net/def/crs/EPSG/0/3049* |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 38N (42°E to 48°E) | ETRS89-TM38N      | *http://www.opengis.net/def/crs/EPSG/0/3050* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 2D TM projection in ETRS89 on GRS80, zone 39N (48°E to 54°E) | ETRS89-TM39N      | *http://www.opengis.net/def/crs/EPSG/0/3051* |
|                                                              |                   |                                              |
| (N,E)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| Height in EVRS                                               | EVRS              | *http://www.opengis.net/def/crs/EPSG/0/5730* |
|                                                              |                   |                                              |
| \(H\)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| Depth referred to LAT                                        | LAT               | *http://www.opengis.net/def/crs/EPSG/0/5861* |
|                                                              |                   |                                              |
| \(D\)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| Depth referred to MSL                                        | MSL               | *http://www.opengis.net/def/crs/EPSG/0/5715* |
|                                                              |                   |                                              |
| \(D\)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| Pressure coordinate in the free atmosphere                   | ISA               | *\<http URI Identifier\>*                    |
|                                                              |                   |                                              |
| \(P\)                                                        |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+
| 3D compound: 2D geodetic in ETRS89 on GRS80, and EVRS height | ETRS89-GRS80-EVRS | *http://www.opengis.net/def/crs/EPSG/0/7409* |
|                                                              |                   |                                              |
| (Latitude, Longitude, H)                                     |                   |                                              |
+--------------------------------------------------------------+-------------------+----------------------------------------------+

5.  ::: {custom-style="Recommendation"}
    As a general rule for referring a compound CRS, one 2D and one 1D system combined together, the respective identifier shall be created by appending the identifiers of the 2D and 1D CRS with a hyphen between both.
    :::

EXAMPLE When both ETRS89-GRS80 and EVRS the CRS used the identifier shall be ETRS89-GRS80-EVRS.

#  Bibliography {#bibliography .list-paragraph}

\[DS-D2.3\] INSPIRE DS-D2.3, Definition of Annex Themes and Scope, v3.0, http://inspire.jrc.ec.europa.eu/reports/ImplementingRules/DataSpecifications/D2.3_Definition_of_Annex_Themes_and_scope_v3.0.pdf

\[DS-D2.5\] INSPIRE DS-D2.5, Generic Conceptual Model, v3.4rc2, *http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/D2.5_v3.4rc2.pdf*

\[DS-D2.6\] INSPIRE DS-D2.6, Methodology for the development of data specifications, v3.0, http://inspire.jrc.ec.europa.eu/reports/ImplementingRules/DataSpecifications/D2.6_v3.0.pdf

\[DS-D2.7\] INSPIRE DS-D2.7, Guidelines for the encoding of spatial data, v3.3rc2, *http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/D2.7_v3.3rc2.pdf*

\[EUR 19575 EN\] Spatial Reference Systems in Europe -- EUR Report 19575 EN. Proceedings of the "Spatial Reference Systems in Europe" workshop, Marne-La Vallee, 29-30 November 1999

\[EUR 20120 EN\] Map Projections for Europe -- EUR Report 20120 EN. Proceedings of the "Map Projections for Europe" workshop, Marne-La Vallee, 14-15 December 2000

> *http://www.ec-gis.org/sdi/publist/pdfs/annoni-etal2003eur.pdf*

\[EUR 21494 EN\] European Reference Grids -- EUR Report 21494 EN. Proceedings of the "European Reference Grids" workshop, Ispra, 27-29 October 2003

> *http://www.ec-gis.org/sdi/publist/pdfs/annoni2005eurgrids.pdf*

\[EUREF\] *www.euref.eu* or *www.euref-iag.net* -- EUREF website for information on the ETRS89 and the EVRS

\[ICAO\] *www.icao.int* *http://www.wmo.int/* -- International Civil Aviation Organization

\[IERS\] *www.iers.org* -- IERS website for information on the ITRS

\[IHO\] *www.iho.int* -- IHO website for publications and information on Hydrography

\[IOC\] *ioc-unesco.org* *http://www.wmo.int/* -- Intergovernmental Oceanographic Commission

\[ISO 19111\] EN ISO 19111:2007 Geographic information - Spatial referencing by coordinates (ISO 19111:2007)

\[ISO 19115\] EN ISO 19115:2005, Geographic information -- Metadata (ISO 19115:2003)

\[ISO 19128\] EN ISO 19128: 2008, Geographic information -- Web Map Server Interface (ISO 19128:2005)

\[ISO 19135\] EN ISO 19135:2007 Geographic information -- Procedures for item registration (ISO 19135:2005)

\[GRIB\] (GRIdded Binary) -- WMO operational open data standard for multiple-dimensioned array data, exchanged daily by WMO, ICAO and IOC,

> *http://www.wmo.ch/pages/prog/www/WMOCodes/OperationalCodes.html*

\[NetCDF\] (Network Common Data Form) - Data Exchange Standard of the Climate and Forecasting community,

> *http://www.unidata.ucar.edu/software/netcdf/*

\[Snyder, 1987\] Map Projections -- A Working Manual -- Snyder, John P., Professional Paper 1395, U.S. Geological Survey, 1987

\[ViewServiceTG\] INSPIRE Initial Operating Capability Task Force (IOC-TF): Technical Guidance for the implementation of INSPIRE View Services, 3.1.

\[WMO\] *www.wmo.int* -- World Meteorological Organization

A.  ::: {custom-style="ANNEX"}
    \
    (normative)\
    \
    Abstract Test Suite
    :::

Tests for the requirements on Coordinate Reference Systems included in Commission Regulation (EU) No 1089/2010 and discussed in these Technical Guidelines have been integrated in the ATS section of the common data specifications document template. All thematic data specifications therefore include the relevant tests for the CRS-related requirements in their respective ATS (in Annex A), and specifically the tests in sections A.2.1, A.2.2, A.2.4, A.6.2, A.6.3 and A.9.2 of the common data specifications document template, which are included for the reader's convenience below.

**A.2.1 Datum test**

a\) [Purpose]{.ul}: Verify whether each instance in the data set is given with reference to one of the (geodetic) datums allowed by Commission Regulation No 1089/2010.

c\) [Reference]{.ul}: Annex II Section 1.2 of Commission Regulation No 1089/2010.

b\) [Test Method]{.ul}: Check whether each instance of a spatial object type made available under INSPIRE has been expressed using:

-   the European Terrestrial Reference System 1989 (ETRS89) within its geographical scope; or

-   the International Terrestrial Reference System (ITRS) for areas beyond the ETRS89 geographical scope; or

-   other geodetic coordinate reference systems compliant with the ITRS. Compliant with the ITRS means that the system definition is based on the definition of ITRS and there is a well-established and described relationship between both systems, according to the EN ISO 19111.

NOTE See Section 5.3.1 of this document.

**A.2.2 Coordinate reference system test**

a\) [Purpose]{.ul}: Verify whether each instance in the data set is referenced to the three-dimensional, two-dimensional and compound coordinate reference systems allowed by Commission Regulation No 1089/2010.

b\) [Reference]{.ul}: Annex II Section 1.3 of Commission Regulation 1089/2010.

c\) [Test Method]{.ul}: Inspect whether the horizontal and vertical components of coordinates are referenced to one of the following coordinate reference system:

-   Three-dimensional Cartesian coordinates based on a datum specified in 1.2 and using the parameters of the Geodetic Reference System 1980 (GRS80) ellipsoid.

-   Three-dimensional geodetic coordinates (latitude, longitude and ellipsoidal height) based on a datum specified in 1.2 and using the parameters of the GRS80 ellipsoid.

-   Two-dimensional geodetic coordinates (latitude and longitude) based on a datum specified in 1.2 and using the parameters of the GRS80 ellipsoid.

-   Plane coordinates using the ETRS89 Lambert Azimuthal Equal Area coordinate reference system.

-   Plane coordinates using the ETRS89 Lambert Conformal Conic coordinate reference system.

-   Plane coordinates using the ETRS89 Transverse Mercator coordinate reference system.

-   For the vertical component on land, the European Vertical Reference System (EVRS) shall be used to express gravity-related heights within its geographical scope. Other vertical reference systems related to the Earth gravity field shall be used to express gravity-related heights in areas that are outside the geographical scope of EVRS.

-   For the vertical component in marine areas where there is an appreciable tidal range (tidal waters), the Lowest Astronomical Tide (LAT) shall be used as the reference surface.

-   For the vertical component in marine areas without an appreciable tidal range, in open oceans and effectively in waters that are deeper than 200 meters, the Mean Sea Level (MSL) or a well-defined reference level close to the MSL shall be used as the reference surface."

-   For the vertical component in the free atmosphere, barometric pressure, converted to height using ISO 2533:1975 International Standard Atmosphere, or other linear or parametric reference systems shall be used. Where other parametric reference systems are used, these shall be described in an accessible reference using EN ISO 19111-2:2012.

NOTE See Section 5.4 of this document.

**A.2.4 View service coordinate reference system test**

a\) [Purpose]{.ul}: Verify whether the spatial data set is available in the two dimensional geodetic coordinate system for their display with the INSPIRE View Service.

b\) [Reference]{.ul}: Annex II Section 1.4 of Commission Regulation 1089/2010.

c\) [Test Method]{.ul}: Check that each instance of a spatial object type in a data set delivered for INSPIRE is available in the two-dimensional geodetic coordinate system.

NOTE See Section 5.4.1 of this document.

**A.6 Information Accessibility Conformance Class**

**A.6.2 CRS publication test**

a\) [Purpose]{.ul}: Verify whether the identifiers and the parameters of coordinate reference system are published in common registers.

b\) [Reference]{.ul}: Annex II Section 1.5 of Commission Regulation 1089/2010.

c\) [Test method]{.ul}: Check whether the identifier and the parameter of the CRS used for the dataset are included in a register.

**A.6.3 CRS identification test**

a\) [Purpose]{.ul}: Verify whether identifiers for other coordinate reference systems than specified in Commission Regulation 1089/2010 have been created and their parameters have been described according to EN ISO 19111 and ISO 19127.

b\) [Reference]{.ul}: Annex II Section 1.3.4 of Commission Regulation 1089/2010.

c\) [Test method]{.ul}: Check whether the register with the identifiers of the coordinate reference systems is accessible.

NOTE Further technical information is given in section 6 of this document.

**A.9 Technical Guideline Conformance Class**

**A.9.2 CRS http URI test**

a\) [Purpose]{.ul}: Verify whether the coordinate reference system used to deliver data for INSPIRE network services has been identified by URIs according to the EPSG register.

c\) [Reference]{.ul}: Table 1 in Section 5.5 of these Technical Guidelines.

b\) [Test Method]{.ul}: Compare the URI of the dataset with the URIs in the table.

NOTE 1 Passing this test implies the fulfilment of test A.2.1

NOTE 2 Further reference please see *http://www.epsg.org/geodetic.html*

[^1]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} The common document template is available in the "Framework documents" section of the data specifications web page at [[http://inspire.jrc.ec.europa.eu/index.cfm/pageid/2]{custom-style="Hyperlink"}](http://inspire.jrc.ec.europa.eu/index.cfm/pageid/2)
    :::

[^2]: ::: {custom-style="footer"}
    []{custom-style="footnote reference"} For all 34 Annex I,II and III data themes: within two years of the adoption of the corresponding Implementing Rules for newly collected and extensively restructured data and within 5 years for other data in electronic format still in use
    :::

[^3]: ::: {custom-style="HTML Preformatted"}
    [ ]{custom-style="footnote reference"}The current status of registered SDICs/LMOs is available via INSPIRE website: [[http://inspire.jrc.ec.europa.eu/index.cfm/pageid/42]{custom-style="Hyperlink"}](http://inspire.jrc.ec.europa.eu/index.cfm/pageid/42)
    :::

[^4]: ::: {custom-style="footer"}
    [ ]{custom-style="footnote reference"}Surveys on unique identifiers and usage of the elements of the spatial and temporal schema,
    :::

[^5]: ::: {custom-style="footer"}
    [ ]{custom-style="footnote reference"}The Data Specification Drafting Team has been composed of experts from Austria, Belgium, Czech Republic, France, Germany, Greece, Italy, Netherlands, Norway, Poland, Switzerland, UK, and the European Environment Agency
    :::

[^6]: ::: {custom-style="footer"}
    []{custom-style="footnote reference"} The Thematic Working Groups of Annex II and III themes have been composed of experts from Austria, Belgium, Bulgaria, Czech Republic, Denmark, Finland, France, Germany, Hungary, Ireland, Italy, Latvia, Netherlands, Norway, Poland, Romania, Slovakia, Spain, Sweden, Switzerland, Turkey, UK, the European Commission, and the European Environment Agency
    :::

[^7]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} For Annex II+III, the consultation and testing phase lasted from 20 June to 21 October 2011.
    :::

[^8]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} [Commission Regulation (EU) No 1089/2010]{custom-style="Strong"} [[implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services,]{custom-style="Hyperlink"}](http://eur-lex.europa.eu/JOHtml.do?uri=OJ:L:2010:323:SOM:EN:HTML) [published in the Official Journal of the European Union on 8^th^ of December 2010.]{custom-style="Strong"}
    :::

[^9]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} The framework documents are available in the "Framework documents" section of the data specifications web page at [[http://inspire.jrc.ec.europa.eu/index.cfm/pageid/2]{custom-style="Hyperlink"}](http://inspire.jrc.ec.europa.eu/index.cfm/pageid/2)
    :::

[^10]: ::: {custom-style="footer"}
    [ ]{custom-style="footnote reference"}UML -- Unified Modelling Language
    :::

[^11]: ::: {custom-style="footer"}
    []{custom-style="footnote reference"} Conceptual models related to specific areas (e.g. INSPIRE themes)
    :::

[^12]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} In the case of the Annex II+III data specifications, the extracted requirements are used to formulate an amendment to the existing Implementing Rule.
    :::

[^13]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} like barometric, or other systems
    :::

[^14]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} The workshop took place on 15/12/2000. See proceedings on [[http://www.ec-gis.org/sdi/publist/pdfs/annoni-etal2003eur.pdf]{custom-style="Hyperlink"}](http://www.ec-gis.org/sdi/publist/pdfs/annoni-etal2003eur.pdf)
    :::

    ::: {custom-style="footnote text"}
    [[http://www.ec-gis.org/sdi/publist/pdfs/annoni-etal2003eur.pdf]{custom-style="Hyperlink"}](http://www.ec-gis.org/sdi/publist/pdfs/annoni-etal2003eur.pdf)
    :::

[^15]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} OJ L 274, 20.10.2009, p. 9--18.
    :::

[^16]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} The INSPIRE Glossary is available from http://inspire-registry.jrc.ec.europa.eu/registers/GLOSSARY
    :::

[^17]: ::: {custom-style="annotation text"}
    []{custom-style="footnote reference"} See []{custom-style="annotation reference"}Geodetic Reference System 1980, Bulletin Géodésique, Vol 54:3, 1980. Republished (with corrections) in Moritz, H., 2000, Geodetic Reference System 1980, J. Geod., 74(1), pp. 128-162, doi:10.1007/S001900050278.[]{custom-style="annotation reference"}
    :::

[^18]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} OJ L 274, 20.10.2009, p. 9--18.
    :::

[^19]: ::: {custom-style="footnote text"}
    []{custom-style="footnote reference"} In 1951, the International Civil Aviation Organisation (ICAO) incorporated the International Standard Atmosphere (ISA) into international law under Annex 8 of the Convention on International Civil Aviation (the Chicago Convention, 1947). ISO adopted the Standard Atmosphere as ISO 2533:1975 in the range 2km to 32km (Manual of the ICAO Standard Atmosphere: Doc 7488/3).
    :::