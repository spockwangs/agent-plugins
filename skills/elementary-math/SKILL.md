---
name: elementary-math
description: Design elementary mathematics lessons, worksheets, and print-quality Chinese PDF materials using first-principles explanations, age-appropriate visual models, guided discovery, and layered practice. Use when teaching primary-school math, creating visual math exercises, explaining arithmetic laws conceptually, or producing Chinese LaTeX worksheets and answer keys.
---

# Elementary Mathematics

Create materials that help children understand why mathematics works before asking them to memorize rules.

## Teaching principles

1. Start from concrete actions or invariant relationships, not a formula.
2. Move through this sequence:
   - concrete situation or action;
   - visual model;
   - spoken explanation;
   - numerical examples;
   - symbolic generalization;
   - application.
3. Ask children to observe, compare, predict, draw, and explain.
4. Introduce formal terminology only after examples reveal the pattern.
5. Keep numbers and language appropriate for the intended grade.
6. Distinguish a calculation result from the reason it is valid.

## Visual models

Choose the model that exposes the mathematical structure:

- number line: addition/subtraction as directed movement and distance;
- counters or ten-frames: composition, decomposition, and place value;
- bar model: part-whole and comparison relationships;
- array or area model: multiplication, division, and distributivity;
- geometric transformation: symmetry, congruence, and spatial reasoning.

The diagram must carry explanatory meaning. Label the start, action, quantity, and result when relevant. Do not add decorative graphics that compete with the mathematics.

## Guided-discovery pattern

When introducing a law or property:

1. Show at least two small examples.
2. Represent both sides with the same visual model.
3. Ask what changed and what stayed invariant.
4. Let the learner state the pattern in words.
5. Present the symbolic form.
6. Include a non-example or common misconception.
7. Apply the property in a purposeful calculation.

For addition:

- Interpret \(a+b\) as starting at \(a\) and moving \(b\) units right on a number line.
- Derive \(a+b=b+a\) by comparing two routes with the same total lengths in opposite order.
- Derive \((a+b)+c=a+(b+c)\) by regrouping the same three consecutive lengths.
- Explicitly distinguish changing order from changing grouping.
- Explain \(a+0=a\) as a movement of zero units.

## Exercise design

Build a progression rather than a list of near-duplicate calculations:

1. read or complete a visual example;
2. draw the model from a given expression;
3. write an expression from a model or story;
4. fill a missing value;
5. compare two representations without calculating;
6. explain why a statement is true;
7. diagnose an incorrect argument;
8. apply the idea to simplify a calculation;
9. solve an open-ended task with multiple valid answers.

Use enough blank space for drawing and written reasoning. Provide answers and short reasoning for conceptual questions. Keep the answer key separate from student pages when practical.

## Simplifying calculations

Teach "friendly numbers" as a consequence of the laws, not as an unexplained trick:

1. identify a pair that forms a convenient total such as \(10\) or \(100\);
2. use commutativity to place the pair together if needed;
3. use associativity to calculate that pair first;
4. annotate which law justifies each transformation.

Do not accept a correct total paired with an invalid transformation.

## Chinese print-quality PDF workflow

Use XeLaTeX with `ctexart`, `amsmath`, and TikZ for editable vector diagrams.

Default typography:

- A4 page with comfortable margins;
- body text in regular Kaiti, without bold emphasis;
- reserve bold sans-serif for the title, section headings, and box headings;
- use LaTeX math mode for all mathematical symbols and formulas;
- use restrained, high-contrast colors that remain readable when printed;
- avoid splitting an example, diagram, or conclusion across pages.

Locate an installed Kaiti font instead of assuming a font name resolves in every environment. Prefer an explicit font file path when compilation is sandboxed. Keep Latin and mathematics fonts separate from the CJK body font.

Use semantic visual hierarchy:

- blue or neutral boxes for core ideas;
- green boxes for observations;
- orange boxes for formal conclusions;
- consistent colors for the same movement or quantity across related diagrams.

## Required validation

Before delivering a PDF:

1. compile with XeLaTeX twice so page references stabilize;
2. check for compilation errors, missing glyphs, and overfull boxes;
3. render pages to images and visually inspect:
   - Chinese font and weight;
   - diagram labels and arrows;
   - clipping and overlap;
   - page breaks;
   - answer space;
   - page count and footer references;
4. revise and rebuild until the visual checks pass;
5. remove temporary previews and auxiliary build files;
6. deliver both the PDF and editable `.tex` source unless the user requests otherwise.

## Quality checklist

- [ ] The concept begins with meaning, not a memorized procedure.
- [ ] Every diagram supports a specific inference.
- [ ] Examples lead naturally to the symbolic statement.
- [ ] Rules are accompanied by a reason or invariant.
- [ ] Exercises progress from representation to explanation and transfer.
- [ ] Common misconceptions are addressed.
- [ ] Body text is regular Kaiti and not bold.
- [ ] Mathematical notation is typeset consistently.
- [ ] The PDF has been compiled and visually inspected.
