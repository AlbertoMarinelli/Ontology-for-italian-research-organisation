# Ontology for italian research organization

Project for the Semantic Web course @ [University of Pisa](https://www.unipi.it/index.php/english)

<img src="imgs/unipi_logo.png" align="right" alt="Unipi logo">

Authors: [Alberto Marinelli](https://github.com/AlbertoMarinelli)


### Ontology Description
This **ontology** had to represent the fundamental concepts of an application domain relating to an **Italian research organisation**, which are: employees, institutes, laboratories and research groups. Some of the facts that characterise this domain can be stated as follows:
1. An employee is a person who has exactly one contract with the research organisation.
2. An employee can be a researcher, a technologist, a graduate fellow, a postdoctoral fellow or a member of the administrative staff.
3. A researcher can be a young researcher, a senior researcher or a director.
4. Each employee has a unique ID (an positive integer).
5. A research organisation has three types of subparts: institute, laboratory and research group. The research organisation consists of more than one institute, each institute consists of more than one laboratory, and each laboratory consists of at least one research group.
6. Each institute, each laboratory and each research group have exactly one name (a string).
7. Each institute is identified by an ID number (a positive integer) and the date of its creation.
8. Each institute has exactly one institute director.
9. Each researcher, technologist, graduate fellow or postdoctoral fellow is member of exactly one laboratory and exactly one research group.
10. Each institute has one or more buildings. Each building has exactly one location. Each building contains more than one office.
11. Each employee has exactly one office. Each office hosts one or more employees.
12. Research organisation, employee, institute, laboratory, research group, building, location and office are pairwise disjoint concepts.
<br>
All the above statements are expressed in an **OWL 2 DL** ontology, using the **RDF Turtle** notation.
In addition, the ontology has the following requirements:<br>
Q1. Declare the required classes, providing for each class a textual label and a concise textual description of the intension of the class, using the appropriate annotation properties from the RDF Schema vocabulary<br>
Q2. Provide the sub-class axioms defining the class taxonomy<br>
Q3. Declare the required object properties, providing for each property:<br>
  Q3.1. a textual label, using the appropriate annotation property from the RDFS vocabulary<br>
  Q3.2. a textual description of the intension of the property, using the appropriate annotation property from the RDFS vocabulary<br>
  Q3.3. one axiom defining the domain of the property<br>
  Q3.4. one axiom defining the range of the property
  Q3.5. one axiom defining the inverse of the property
  Q3.6. any additional axioms expressing disjointness of the property with other object properties, and the property characteristics.
Q4. Provide the sub-property axioms defining the object property taxonomy
Q5. Declare the required data properties, providing:
  Q5.1. a textual label, using the appropriate annotation property from the RDFS vocabulary
  Q5.2. a textual description of the intension of the property, using the appropriate annotation property from the RDFS vocabulary
  Q5.3. one axiom defining the domain of the property
  Q5.4. one axiom defining the range of the property
  Q5.5. any additional axioms expressing disjointness of the property with other data properties, and whether the property is functional.
Q6. Define the axioms necessary for expressing any statement in 1 to 12 that has not already been expressed.
Q7. Populate the ontology with at least one individual for each class, and at least one assertion for each property.
