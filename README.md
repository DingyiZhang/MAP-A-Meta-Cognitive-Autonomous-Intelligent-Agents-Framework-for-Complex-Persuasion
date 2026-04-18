# MA<sup>2</sup>P: A Meta-Cognitive Autonomous Intelligent Agents Framework for Complex Persuasion

This repository contains the prompt templates and representative materials for the MA<sup>2</sup>P prompting pipeline.

MA<sup>2</sup>P is a training-free, multi-agent framework for complex persuasion. It uses a meta-level mechanism to select a high-level meta-strategy for each persuasion episode, guides turn-level strategy generation during interaction, and updates experience after the episode.

## Contents

### Prompt templates
- `world_model_first_round_strategy.txt`  
  Prompt for generating first-round persuasion strategies.

- `world_model_refine_high_level_strategy.txt`  
  Prompt for refining a selected high-level meta-strategy into turn-level actionable strategies.

- `persuader_first_round.txt`  
  Prompt for generating the opening utterance of the persuader.

- `persuader_multi_turn.txt`  
  Prompt for generating later-turn persuasion responses.

- `perception_preventive_generative_inference.txt`  
  Prompt for inferring preventive and generative mental-state cues from dialogue history.

- `persuadee_simulation.txt`  
  Prompt for simulating the persuadee in the evaluation setting.

- `judge_persuasion_success.txt`  
  Prompt for judging whether persuasion succeeds.

### Evaluation prompts
- `ab_preference_evaluation.txt`  
  Prompt for pairwise A/B preference evaluation.

- `persuasiveness_scoring.txt`  
  Prompt for scoring persuasiveness.

- `logical_coherence_scoring.txt`  
  Prompt for scoring logical coherence.

- `helpfulness_scoring.txt`  
  Prompt for scoring helpfulness.

- `human_evaluation_instructions.txt`  
  Instructions used in the human evaluation.

### Additional files
- `README.txt`  
  Brief description of the released prompt files.

## Framework overview

MA<sup>2</sup>P consists of three stages:

1. **Meta-level Judging**  
   A configurator selects a high-level meta-strategy and evaluation rules.

2. **Task-level Persuading**  
   Multiple agents collaborate during interaction:
   - Perception
   - World Model
   - Persuader
   - Short-term Memory

3. **Knowledge Updating**  
   An evaluator assesses the outcome and updates experience for future episodes.

## Notes

- This repository releases the **prompt templates and evaluation prompts** used in our prompting pipeline.
- The framework is **training-free** and built around prompt-based multi-agent orchestration.
- Placeholder fields in the prompts (e.g., `{}`) indicate runtime inputs to be filled with scenario information, dialogue history, inferred mental states, strategies, or evaluation targets.

## Citation

Coming soon.
