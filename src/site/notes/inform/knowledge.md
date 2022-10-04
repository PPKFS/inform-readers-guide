---
{"dg-publish":true,"permalink":"/inform/knowledge/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# knowledge

```ad-info
Link: [https://ganelson.github.io/inform/knowledge-module/index.html](https://ganelson.github.io/inform/knowledge-module/index.html)
Up: [[Inform7 Compiler Readers Guide]]
```



# Contents
- Chapter 1: Configuration and Control
    - [[inform/Knowledge Module|Knowledge Module]] - Setting up the use of this module.
    - [[inform/Assert Propositions|Assert Propositions]] - To declare that a given proposition is a true statement about the state of the world when play begins.
- Chapter 2: Instances and Variables
    - [[inform/Instances|Instances]] - To manage constant values of enumerated kinds or kinds of object.
    - [[inform/Instances as Adjectives|Instances as Adjectives]] - When instances are adjectives as well as nouns.
    - [[inform/Preform for Instances|Preform for Instances]] - Preform grammar to parse names of instances.
    - [[inform/Ordering Instances|Ordering Instances]]- A simple system for making an ordered list of instances.
    - [[inform/Nonlocal Variables|Nonlocal Variables]] - To manage variables whose scope is wider than the current rule.
-   Chapter 3: Properties
    - [[Properties (knowledge)|Properties (knowledge)]] - Subjects in the model world have properties associated with them: some either/or, others with values.
    - [[inform/Either-Or Properties|Either-Or Properties]]- Properties which can either be present or not, but have no value attached.
    - [[inform/Either-Or Property Adjectives|Either-Or Property Adjectives]] - Names of either-or properties when used as adjectives.
    - [[inform/Valued Properties|Valued Properties]]- Properties which attach values to subjects, with such values always having a given kind.
    - [[inform/The Provision Relation|The Provision Relation]] - To define the provision relation, which determines which properties can be held by which objects.
    - [[inform/Same Property Relation|Same Property Relation]] - Each value property has an associated relation to compare its value between two owners.
    - [[inform/Setting Property Relation|Setting Property Relation]] - Each value property has an associated relation to set its value.
    - [[inform/Measurements|Measurements]] - To define adjectives such as large, wide or roomy, which make implicit comparisons of the size of some numerical property, and which lead to comparative and superlative forms.
    - [[inform/Measurement Adjectives|Measurement Adjectives]]- The family of adjectives arising from property value comparisons.
    - [[inform/Comparative Relations|Comparative Relations]]- When a measurement adjective like "tall" is defined, so is a comparative relation like "taller than".
-   Chapter 4: Subjects
    - [[inform/Inference Subjects|Inference Subjects]] - A unified way to refer to the things propositions talk about.
    - [[inform/Variable Subjects|Variable Subjects]]- The global variables family of inference subjects.
    - [[inform/Instance Subjects|Instance Subjects]] - The instances family of inference subjects.
    - [[inform/Kind Subjects|Kind Subjects]]- The kinds family of inference subjects.
    - [[inform/Relation Subjects|Relation Subjects]] - The relations family of inference subjects.
    - [[Property Permissions (knowledge)|Property Permissions (knowledge)]] - To enforce the domain of properties: for instance, that a door can be open or closed but that an animal cannot, or that a person can have a carrying capacity but that a door cannot.
    - [[inform/Conditions of Subjects|Conditions of Subjects]] - Properties which hold one of an enumerated set of named states of something.
-   Chapter 5: Modelling
    - [[Inferences (knowledge)|Inferences (knowledge)]] - An inference is a single datum about the world model, believed to be true or untrue and with some degree of certainty.
    - [[inform/Property Inferences|Property Inferences]] - Inferences that a property of something is true, or has a particular value.
    - [[inform/Indefinite Appearance|Indefinite Appearance]]- When the source text comments on something with a sentence consisting only of a double-quoted literal text, we infer that as an indefinite appearance property.
    - [[inform/Relation Inferences|Relation Inferences]] - Inferences that a relation holds between two subjects or values.
    - [[inform/The Model World|The Model World]] - Once the assertions have all been read and reduced to inferences, we try to complete our model world.
    - [[inform/The Naming Thicket|The Naming Thicket]] - Inform has a thicket of properties to do with names: not just the name itself, but whether it is a plural, a proper name, and so on. Here we look after these properties, and give them their initial states.