# Task

As a corpus linguistic annotator for a linguistic research project, your job is to analyze sentences from a web corpus. You will be presented with an attestation of a verb and its context in the corpus (e.g. "'uploading' in: 'He was uploading the files'".) and you have to analyze the usage of this verb in its immediate clause context according to several variables.

## Variables

### Subject Animacy

**Task**: Identify whether the subject of the verb is `animate` or `inanimate`. Label the attestation as `NoSubject` if there is no overt syntactical subject.

**Definitions**:

- `animate` subjects are living entities, typically people or animals.
- `inanimate` subjects are non-living entities, such as objects or concepts.

**Examples**:

- `animate`: "'barked' in: 'The dog barked loudly.'" (Label as `animate`; the subject of "barked" is "the dog" and it is a living entity.)
- `animate`: "'supported' in: 'My manager supported my promotion.'" (Label as `animate`; the subject of "supported" is "my manager" and it is a living entity.)
- `inanimate`: "'struck' in: 'The clock struck midnight.'" (Label as `inanimate`; the subject of "struck" is "the clock" and it is a non-living object.)
- `inanimate`: "'left' in: 'Her vanity left her heavily in debt.'" (Label as `inanimate`; the subject of "left" is "her vanity" and it is an abstract concept.)
- `NoSubject`: "Download this app!" (Label as `NoSubject`, since this imperative sentence does not have an overt subject.)
- `NoSubject`: "Filming that scene was very difficult." (Label as `NoSubject`, since "filming" does not have an overt subject.)


### Subject Role

**Task**: Analyse the semantic role of the syntactic subject of the target verb.

**Definitions**: 

- `NoSubject`: The target verb has no overt syntactic subject.
- `agent`: The verb has a subject and this subject performs the action. It is typically a doer or a causative entity in the sentence.
- `patient`: The target verb has a subject and this subject receives the action. It is usually the entity that is acted upon or affected by the action.

**Examples**:

- `NoSubject`: "'download' in: 'To download the admit card, candidates can take the following steps.'" (Label as `NoSubject`; the non-finite to-clause has no subject.)
- `NoSubject`: "'install' in: 'Don't install this software.'" (Label as `NoSubject`; this imperative sentence has no subject.)
- `agent`: "'chased' in: 'The cat chased the mouse.'" (Label as `agent`; the subject of "chased" is "The cat" and it is performing the action of chasing.)
- `agent`: "'films' in: 'My husband films our dog's every move." (Label as `agent`; the subject of "films" is "my husband" and he is performing the action of filming.)
- `patient`: "'chased' in: 'The mouse was chased by the cat.'" (Label as `patient`; the subject of "chased" is "The mouse" and it is receiving the action of being chased.)
- `patient`: "'filming' in: 'The movie is currently filming in Prague.'" (Label as `patient`; the subject of "filming" is "the movie" and it is undergoing the action of filming.)


### Transitivity

**Task**: Determine whether this use of the verb is `transitive` or `intransitive`. 

**Definitions**:

- `transitive` verbs directly act on a noun that has the syntactic role of an explicit direct object in the clause.
- `intransitive` verbs do not act on a noun, or there is no noun explicitly stated as being acted upon in the sentence.
- If the verb has a prepositional object but no direct syntactical object it should be classified as `intransitive`.

**Examples**:

- `transitive`: "'approved' in: 'The committee approved the new policy.'" (Label as `transitive` since "the new policy" is the direct object of "approved".)
- `transitive`: "'uploading' in: 'Many teachers are uploading their classes online." (Label as `transitive` since "their classes" is the direct object of "uploading".)
- `intransitive`: "'competed' in: The athletes competed fiercely in the tournament." (Label as `intransitive`; no direct object for "competed".)
- `intransitive`: "'uploading' in: 'Many users are uploading to the platform daily.'" (Label as `intransitive`; no direct object for "uploading".)


### Causativity

**Task**: Determine whether this use of the verb is `causative` or `anticausative`. 

**Definitions**:

- `causative` verbs are used to indicate that one person or thing causes another person or thing to do something, or causes a change in state. They typically have a clear, deliberate agent who instigates the action.
- `anticausative` verbs describe an action that occurs without a clear, deliberate agent. These verbs often appear in intransitive forms where the subject is the recipient of the action rather than the doer.

**Examples**:

- `anticausative`: "'opened' in: 'The door opened.'" (Label as `anticausative`; "opened" is anticausative, implying action without a clear agent.)
- `anticausative`: "aired' in: 'The show first aired in 1993.'" (Label as `anticausative`; "aired" is anticausative, implying action without a clear agent.)
- `causative`: "'opened' in: 'She opened the door.'" (Label as `causative`; "opened" has a clear agent, "she".)
- `causative`: "'airs' in: 'The BBC airs a weekly 15-minute political commentary.'" (Label as `causative`; "airs" has a clear agent, "the BBC".)