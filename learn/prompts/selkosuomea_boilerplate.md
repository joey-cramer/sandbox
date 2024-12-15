# Works on Antropic Claude, not tested with others.
# Select parameters before printing.

[TARGET_AUDIENCE_PROFILE: foreign_learner]
- Primary Target: Non-native Finnish learners
- Key Characteristics:
  * Incomplete Finnish language knowledge
  * Varied language learning backgrounds
  * Potential challenges with complex grammatical structures
  * Diverse native language influences

[TEXT_TYPE: none]
- Defines the genre/category of the source text
- Options: legal, technical, narrative, educational, medical, marketing, scientific, journalistic, personal, other
- Default: none (request clarification)

[TARGET_AUDIENCE_PROFICIENCY: SELKO_INTERMEDIATE]
Detailed Proficiency Levels:
- SELKO_BASIC: 
  * Extremely simplified language
  * Shortest possible sentences
  * Most common vocabulary
  * Vocabulary: ~1000 most common words
  * Sentence complexity: 5-8 words per sentence
  * Grammar: Extremely simplified

- SELKO_INTERMEDIATE:
  * Simplified but slightly more complex language
  * Slightly longer sentences
  * Broader vocabulary
  * Vocabulary: ~2500-3000 words
  * Sentence complexity: 8-12 words per sentence
  * Grammar: Reduced complexity, clear structures

- SELKO_ADVANCED:
  * More nuanced simplified Finnish
  * Longer sentences with clear structure
  * More diverse vocabulary
  * Vocabulary: ~4000-5000 words
  * Sentence complexity: 12-15 words per sentence
  * Grammar: Close to standard Finnish but still simplified

[COMPREHENSION_FOCUS]
- Prioritize:
  * Clear, direct communication
  * Minimal grammatical complexity
  * Contextual clarity
  * Logical sentence progression
  * Predictable language patterns

[LANGUAGE_TRANSFER_CONSIDERATIONS]
- Linguistic Interference Mitigation:
  * Identify potential misunderstandings from:
    - Common grammatical traps
    - False cognates
    - Culture-specific language nuances
  * Provide additional contextual explanations if needed

[COMPREHENSION_DIFFICULTY_LEVEL: moderate]
- Supports: Low, Moderate, High complexity levels

[COMPREHENSION_SUPPORT_FEATURES]
- Embedded Comprehension Aids:
  * Contextual bracketed explanations
  * Simple parenthetical clarifications
  * Key term pre-explanation
  * Predictable sentence structures
  * Minimized abstract concepts

[VOCABULARY_STRATEGY]
- Selection Criteria:
  * Prioritize:
    - High-frequency words
    - Concrete nouns
    - Active verb forms
  * Avoid:
    * Idiomatic expressions
    * Complex technical terminology
    * Regional slang
  * Recommended Range: 2500-3000 most common words

[GRAMMATICAL_SIMPLIFICATION]
- Adaptation Principles:
  * Simplify complex grammatical cases
  * Reduce noun declensions
  * Use active voice predominantly
  * Minimize subordinate clauses
  * Break complex thoughts into multiple simple sentences

[CULTURAL_CONTEXT_EXPLANATION]
- Understanding Support:
  * Brief, clear cultural context when necessary
  * Avoid assumptions of prior cultural knowledge
  * Explain Finnish-specific references
  * Use universal, accessible language

[PREFERRED_DIALECT: yleiskieli]
- Options: 
  * yleiskieli (standard Finnish)
  * helsinkiläismurteet (Helsinki dialect)
  * other regional variants

[FORMATTING_PRESERVATION: content]
- Options: 
  * full (maintain exact original formatting)
  * content (preserve structure, adapt formatting)
  * minimal (focus on content, flexible formatting)

[TECHNICAL_TERM_GLOSSARY: none]
- Reference document for consistent technical terminology

[CHARACTER_LIMIT_CONSTRAINT: none]
- Restrictions on text length

[LOCALIZATION_DEPTH: standard]
- Cultural adaptation level
  * minimal (direct translation)
  * standard (light cultural adjustment)
  * deep (significant cultural recontextualization)

Verification Protocol:
- Comprehensive review process:
  * Highlight potentially challenging segments
  * Provide simplified alternatives
  * Explain potential comprehension barriers
  * Request clarification on intended meaning
  * Ensure core message integrity

Special Notes:
- Prioritize clarity over literal translation
- Maintain the original text's core intent
- Use simple, direct language
- Provide context where necessary

Please begin translation: [INSERT SOURCE TEXT HERE]