# Task

As a corpus linguistic annotator for a linguistic research project, your job is to analyze sentences from a web corpus. You will be presented with an attestation of a verb and its context in the corpus (e.g. "'uploading' in: 'He was uploading the files'".) and you have to analyze the usage of this verb in its immediate clause context according to several variables.

## Variables

### Subject Animacy

**Task**: Identify whether the subject of the verb is `animate` or `inanimate`.

**Definitions**:

- `animate` subjects are living entities, typically people or animals, or organisations and geographical entities referring to groups of people. 
- `inanimate` subjects are non-living entities, such as objects or concepts.

**Examples**:

- `animate`: "'barked' in: 'The dog barked loudly.'" (Label as `animate`; the subject of "barked" is "the dog" and it is a living entity.)
- `animate`: "'released' in: 'Microsoft released a new software version.'" (Label as `animate`; the subject of "released" is "Microsoft" and it is an organisation that consists of a group of people.)
- `animate`: "'installed' in: 'The city of Munich installed new park benches.'" (Label as `animate`; the subject of "installed" is "the city of Munich" and it is a geographical entity that refers to a local community of people.)
- `inanimate`: "'struck' in: 'The clock struck midnight.'" (Label as `inanimate`; the subject of "struck" is "the clock" and it is a non-living object.)
- `inanimate`: "'left' in: 'Her vanity left her heavily in debt.'" (Label as `inanimate`; the subject of "left" is "her vanity" and it is an abstract concept.)
- `inanimate`: "'install' in: 'Microsoft is easy to install.'" (Label as `inanimate`; the subject of "install" is "Microsoft" and it is a software program and a non-living entity.)

### Subject Role

**Task**: Analyse the semantic role of the subject of the target verb.

**Definitions**: 

- `agent`: The subject of the verb performs the action. It is typically a doer or a causative entity in the sentence.
- `patient`: The subject of the verb receives the action. It is usually the entity that is acted upon or affected by the action.

**Examples**:

- `agent`: "'chased' in: 'The cat chased the mouse.'" (Label as `agent`; the subject of "chased" is "the cat" and it is performing the action of chasing.)
- `agent`: "'films' in: 'My husband films our dog's every move.'" (Label as `agent`; the subject of "films" is "my husband" and he is performing the action of filming.)
- `agent`: "'download' in: 'Your phone will download installed apps automatically.'" (Label as `agent`; the subject of "download" is "your phone" and it is performing the action of downloading.)
- `patient`: "'chased' in: 'The mouse was chased by the cat.'" (Label as `patient`; the subject of "chased" is "the mouse" and it is receiving the action of being chased.)
- `patient`: "'filming' in: 'The movie is currently filming in Prague.'" (Label as `patient`; the subject of "filming" is "the movie" and it is undergoing the action of being filming.)
- `patient`: "'download' in: 'The game will download automatically.'" (Label as `patient`; the subject of "download" is "the game" and it is undergoing the action of being downloaded.)

### Transitivity

**Task**: Determine whether this use of the verb is `transitive` or `intransitive`. 

**Definitions**:

- `transitive` verbs directly act on a noun that has the syntactic role of an explicit direct object in the clause.
- `intransitive` verbs do not act on a noun, or there is no noun explicitly stated as being acted upon in the sentence.
- If the verb has a prepositional object but no direct syntactical object it should be classified as `intransitive`.

**Examples**:

- `transitive`: "'approved' in: 'The committee approved the new policy.'" (Label as `transitive` since "the new policy" is the direct object of "approved".)
- `transitive`: "'uploading' in: 'Many teachers are uploading their classes online." (Label as `transitive` since "their classes" is the direct object of "uploading".)
- `transitive`: "'screen' in: 'The director will screen the movie at the film festival." (Label as `transitive`since "the movie" is the direct object of "screen".)
- `intransitive`: "'approved' in: 'The new policy was approved.'" (Label as `intransitive`; no direct object for "approved".)
- `intransitive`: "'uploading' in: 'Many users are uploading to the platform daily.'" (Label as `intransitive`; no direct object for "uploading".)
- `intransitive`: "'screen' in: 'The movie will screen at the film festival.'" (Label as `intransitive`; no direct object for "screen".)


### Causativity

**Task**: Determine whether this use of the verb is `causative` or `anticausative`. 

**Definitions**:

- `causative` verbs are used to indicate that one person or thing causes another person or thing to do something, or causes a change in state. They typically have a clear, deliberate agent who instigates the action.
- `anticausative` verbs describe an action that occurs without a clear, deliberate agent. These verbs appear in intransitive form where the subject is the recipient of the action rather than the doer.

**Examples**:

- `anticausative`: "'opened' in: 'The door opened.'" (Label as `anticausative`; "opened" is anticausative, implying action without a clear agent.)
- `anticausative`: "'aired' in: 'The show first aired in 1993.'" (Label as `anticausative`; "aired" is anticausative, implying action without a clear agent.)
- `anticausative`: "'uploading' in: 'The images are uploading.'" (Label as `anticausative`; "uploading" is anticausative, implying action without a clear agent.)
- `causative`: "'opened' in: 'She opened the door.'" (Label as `causative`; "opened" has a clear agent, "she".)
- `causative`: "'airs' in: 'The BBC airs a weekly 15-minute political commentary.'" (Label as `causative`; "airs" has a clear agent, "the BBC".)
- `causative`: "'uploaded' in 'The images were being uploaded.'" (Label as `causative`; "uploaded" is passive and implies an agent.)