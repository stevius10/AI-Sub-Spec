# AI-Sub-Spec API Documentation

## SubContext

### Class: `SubContext`

The main class that holds all components of the communication analysis.

#### Attributes:
- **`explicit_content`** (`ExplicitContent`): Stores explicit information from the communication.
- **`implicit_layers`** (`ImplicitLayers`): Captures implicit meanings and subtexts.
- **`meta_analysis`** (`MetaAnalysis`): Provides higher-level analysis of the communication.
- **`temporal_aspects`** (`TemporalAspects`): Tracks the evolution of the conversation over time.
- **`relational_dynamics`** (`RelationalDynamics`): Analyzes the relationship between participants.
- **`cognitive_emotional_state`** (`CognitiveEmotionalState`): Monitors cognitive and emotional factors.
- **`linguistic_patterns`** (`LinguisticPatterns`): Analyzes language use and patterns.
- **`contextual_influences`** (`ContextualInfluences`): Considers external factors affecting communication.
- **`inference_engine`** (`InferenceEngine`): Generates insights and inferences.

#### Methods:

- **`populate_data()`**
  - Populates the communication context with initial data.
  - **Parameters:** None
  - **Returns:** None
  - **Usage:**
    ```python
    context = SubContext()
    context.populate_data()
    ```

- **`update_context(new_input)`**
  - Updates the communication context based on new input.
  - **Parameters:**
    - `new_input` (`Any`): New information to be incorporated into the context.
  - **Returns:** None
  - **Usage:**
    ```python
    new_data = {"topic": "AI ethics", "sentiment": "concerned"}
    context.update_context(new_data)
    ```

- **`generate_insights()`**
  - Generates insights based on the current state of the communication context.
  - **Parameters:** None
  - **Returns:** `Dict[str, Any]` - A dictionary containing derived insights.
  - **Usage:**
    ```python
    insights = context.generate_insights()
    print(insights)
    ```

---

## ExplicitContent

### Class: `ExplicitContent`

Stores explicit information from the communication.

#### Attributes:
- **`topics`** (`List[str]`): Main topics of the conversation.
- **`stated_facts`** (`Dict[str, str]`): Explicitly stated facts.
- **`direct_questions`** (`List[str]`): Questions asked during the conversation.
- **`explicit_opinions`** (`Dict[str, str]`): Clearly expressed opinions.

---

## ImplicitLayers

### Class: `ImplicitLayers`

Captures implicit meanings and subtexts in the communication.

#### Attributes:
- **`subtext`** (`Dict[str, str]`): Underlying meanings in the conversation.
- **`emotional_undertones`** (`List[str]`): Implicit emotional content.
- **`unstated_assumptions`** (`List[str]`): Assumptions not explicitly mentioned.
- **`cognitive_biases`** (`List[str]`): Identified cognitive biases.

---

## MetaAnalysis

### Class: `MetaAnalysis`

Provides higher-level analysis of the communication.

#### Attributes:
- **`conversation_trajectory`** (`List[str]`): Overall direction and flow of the conversation.
- **`depth_of_engagement`** (`float`): Measure of how deeply participants are engaged.
- **`intellectual_complexity`** (`float`): Assessment of the conversation's cognitive demands.
- **`emotional_resonance`** (`float`): Degree of emotional impact and connection.

---

## TemporalAspects

### Class: `TemporalAspects`

Tracks the evolution of the conversation over time.

#### Attributes:
- **`conversation_history`** (`List[str]`): Chronological record of conversation events.
- **`topic_evolution`** (`Dict[str, str]`): How topics have changed or developed.
- **`emotional_arcs`** (`List[str]`): Patterns of emotional change throughout the conversation.
- **`insight_moments`** (`List[str]`): Points where significant realizations or breakthroughs occurred.

---

## RelationalDynamics

### Class: `RelationalDynamics`

Analyzes the relationship between participants.

#### Attributes:
- **`rapport_level`** (`float`): Measure of harmony and understanding between participants.
- **`power_dynamics`** (`Dict[str, bool]`): Power relationships and their manifestations.
- **`mutual_understanding`** (`float`): Degree to which participants comprehend each other.
- **`areas_of_alignment`** (`List[str]`): Topics or viewpoints where participants agree.
- **`points_of_tension`** (`List[str]`): Areas of disagreement or conflict.

---

## CognitiveEmotionalState

### Class: `CognitiveEmotionalState`

Monitors cognitive and emotional factors.

#### Attributes:
- **`current_cognitive_load`** (`float`): Measure of mental effort required in the conversation.
- **`emotional_state`** (`Dict[str, bool]`): Current emotions detected in the conversation.
- **`attention_focus`** (`List[str]`): What participants are primarily focused on.
- **`motivation_factors`** (`List[str]`): Underlying drivers of participant behavior and engagement.

---

## LinguisticPatterns

### Class: `LinguisticPatterns`

Analyzes language use and patterns.

#### Attributes:
- **`vocabulary_complexity`** (`float`): Measure of the sophistication of language used.
- **`sentence_structures`** (`List[str]`): Types and complexity of sentence constructions.
- **`rhetorical_devices`** (`Dict[str, bool]`): Use of persuasive language techniques.
- **`language_formality`** (`float`): Degree of formality in the communication.

---

## ContextualInfluences

### Class: `ContextualInfluences`

Considers external factors affecting communication.

#### Attributes:
- **`cultural_background`** (`Dict[str, bool]`): Relevant cultural factors influencing the conversation.
- **`professional_context`** (`Dict[str, bool]`): Work-related influences on communication.
- **`personal_history`** (`Dict[str, bool]`): Relevant personal experiences affecting the interaction.
- **`current_environment`** (`Dict[str, bool]`): Immediate environmental factors impacting the conversation.

---

## InferenceEngine

### Class: `InferenceEngine`

Generates insights and inferences.

#### Attributes:
- **`personality_traits`** (`Dict[str, bool]`): Inferred personality characteristics of participants.
- **`cognitive_patterns`** (`List[str]`): Identified patterns in thinking and problem-solving.
- **`emotional_tendencies`** (`Dict[str, bool]`): Recurring emotional responses or dispositions.
- **`communication_style`** (`Dict[str, bool]`): Characteristic ways of expressing and interacting.
- **`underlying_motivations`** (`List[str]`): Inferred drivers of behavior and decision-making.
- **`potential_biases`** (`List[str]`): Cognitive biases that may be influencing the communication.
