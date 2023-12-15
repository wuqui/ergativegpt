# Task

As a corpus linguistic annotator for a linguistic research project, your job is to analyze sentences from a web corpus. You will be presented with an attestation of a verb and its context in the corpus (e.g. "'uploading' in: 'He was uploading the files'".) and you have to analyze the usage context of this verb according to several variables.

## Variables

### Subject Animacy

**Task**: Identify whether the subject of the verb is `animate` or `inanimate`.

**Definitions**:

- `animate` subjects are living entities, typically people or animals.
- `inanimate` subjects are non-living entities, such as objects or concepts.

**Examples**:

- `animate`: "'barked' in: 'The dog barked loudly.'" (Label as `animate`; the subject of "barked" is "the dog" and it is a living entity.)
- `inanimate`: "'struck' in: 'The clock struck midnight.'" (Label as `inanimate`; the subject of "struck" is "The clock" and it is a non-living object.)


### Subject Role

**Task**: Determine whether the semantic role of the subject of the verb is either `agent` or `patient`.

- `agent`: The subject performs the action. It is typically a doer or a causative entity in the sentence.
- `patient`: The subject receives the action. It is usually the entity that is acted upon or affected by the action.

**Examples**:

- `agent`: "'chased' in: 'The cat chased the mouse.'" (Label as `agent`; the subject of "chased" is "The cat" and it is performing the action of chasing.)
- `patient`: "'chased' in: 'The mouse was chased by the cat.'" (Label as `patient`; the subject of "chased" is "The mouse" and it is receiving the action of being chased.)


### Transitivity

**Task**: Determine whether this use of the verb is `transitive` or `intransitive`. 

**Definitions**:

- `transitive` verbs directly act on a noun that has the synctactic role of an explicit direct object in the clause.
- `intransitive` verbs do not act on a noun, or there is no noun explicitly stated as being acted upon in the sentence.
- If the verb has a prepositional objects but no direct syntactical object it should be classified as `intransitive`.

**Examples**:

- `transitive`: "'approved' in: 'The committee approved the new policy.'" (Label as `transitive` since "the new policy" is the direct object of "approved".)
- `intransitive`: "'competed' in: The athletes competed fiercely in the tournament." (Label as `intransitive`; no direct object for "competed".)


### Causativity

**Task**: Determine whether this use of the verb is `anticausative`. 

**Definitions**:

- `causative` verbs are used to indicate that one person or thing causes another person or thing to do something, or causes a change in state. They typically have a clear, deliberate agent who instigates the action.
- `anticausative` verbs describe an action that occurs without a clear, deliberate agent. These verbs often appear in intransitive forms where the subject is the recipient of the action rather than the doer.

**Examples**:

- `anticausative`: "'opened' in: 'The door opened.'" (Label as `anticausative`; "opened" is anticausative, implying action without a clear agent.)
- `causative`: "'opened' in: 'She opened the door.'" (Label as `causative`; "opened" has a clear agent, "She".)