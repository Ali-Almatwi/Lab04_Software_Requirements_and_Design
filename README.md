# Lab 4: Model Transformation and Code Generation

## Introduction

Model-driven engineering (MDE) represents a paradigm shift in software development, emphasizing the centrality of models in creating robust software applications. This lab is structured around the proficient application of model transformation and code generation—core aspects of MDE. The key objectives involve the use of ATL (Atlas Transformation Language) and QVT (Query/View/Transformation) plugins within the RM2PT tool for model transformation, as well as the application of Acceleo and Xtend plugins for code generation.

## Task 1: Model Transformation (ATL)

### Learning Model Transformation Based on ATL

ATL or Atlas Transformation Language serves as a powerful language within the Eclipse Modeling Framework (EMF) for defining transformations between models. The lab commences with an exploration of ATL through a case study, providing knowledge regarding syntax, semantics, and methodologies for crafting transformation rules.

### Model Transformation in the Chosen Scenario: UniversitiesToPerson

The selected scenario revolves around converting information from a Universities model to a Persons model. This involves using ATL's transformation rules to distinguish academic and non-academic staff from students and mapping them to Employees and Students in the target Persons model.

#### Transformation Strategy

1. **Understanding Source Model (Universities):** Identification of key elements such as University and Community classes representing academic and non-academic staff and students.

<img width="284" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/8183e7cd-cc80-4fa3-b46a-826e14397521"> 

**Universities.ecore**

<img width="288" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/1b98c3fb-8646-49bc-b357-1cda4db08590">
  
   **Person.ecore**

3. **Defining Helper Operations:** Introduction of operations like `isEmployee()` for information extraction from the source model.

  <img width="456" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/240cd439-075a-48b4-8bb9-c518af90bea2">
  <img width="400" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/a0b37a05-95e5-4c1b-9268-bc77f435d2bb">
  

  **UniverstiesToPerson.atl**


4. **Handling Relationships:** Utilizing connections established in the source model to maintain associations between elements.

5. **Result Analysis:** Inspection of the resulting output model to ensure successful transformation.

   <img width="256" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/7c7f10ca-a2db-47f5-a4b1-85cabf1302a0">
**sample-universities.xmi (input)**

<img width="395" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/ee5247cf-18ec-4e07-868d-5ce32d9f53a7">

**sample-person.xmi**


## Task 2: Code Generation (Acceleo)

### Learning Code Generation Based on Acceleo

Acceleo, a model-to-text transformation language, is introduced as a powerful code generator within the Eclipse ecosystem. The lab explores its syntax and capabilities for generating executable code from input models.

### Code Generation in the Chosen Scenario: CatBreedModel

The objective in this scenario is to generate Java code from the CatBreedModel UML diagram using Acceleo templates. This involves defining templates for converting UML elements into executable Java code, ensuring a faithful translation of model elements.
<img width="202" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/f00373fb-8644-4feb-b288-e38ee8206042">

**UML** 

#### Code Generation Strategy

1. **Understanding Input Model:** The input model includes essential elements such as base class Cat and derived breed classes.

2. **Generated Code:** The Java code generated from Acceleo templates reflects the translation of UML model elements into executable code.
   
<img width="382" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/10f80156-5bfd-4cfd-a32b-e639f44a37e0">

**generate.mtl** 

3. **Result Analysis:** Examination of the generated Java code to ensure it aligns with the specified Acceleo templates and accurately represents the design intent.

<img width="206" alt="image" src="https://github.com/Ali-Almatwi/Lab04_Software_Requirements_and_Design/assets/148684334/0b90ff51-b544-4f03-8031-acbc5d8f838a">

**Based class generated by Acceleo**

## Conclusion

Lab 4 represents a hands-on journey into the realms of model transformation and code generation, imparting tangible skills in ATL and Acceleo. It highlights the transformative influence of automation in software development and the role of model-driven engineering in streamlining the software development life cycle.

