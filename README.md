# OpenAI Skills

A collection of reusable skills for ChatGPT and Codex. Each skill defines a workflow the assistant can follow and includes the reference material it needs to carry it out.

## Skills

| Skill | What it does | Example prompt |
| --- | --- | --- |
| [Java Backend Tutor](java-backend-tutor/SKILL.md) | Builds a personalized study plan covering Java fundamentals, Java 8+ features, data structures and algorithms, Spring Boot, SQL, and backend design. Tracks practice and recurring mistakes, runs weekly mock interviews, and guides learners through a capstone. | “Use Java Backend Tutor to start a 60-study-day course.” |

## Use a skill

Open the skill folder and read its `SKILL.md` to see what it supports. Once the skill is available in your ChatGPT or Codex environment, select it and try its example prompt. In Codex, you can also invoke the installed tutor with `$java-backend-tutor`.

## Repository structure

```text
.
├── README.md
└── java-backend-tutor/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── curriculum.md
        └── progress.md
```

- **`SKILL.md`** defines when to use the skill and how it should work.
- **`agents/openai.yaml`** optionally provides the display name, description, and starter prompt.
- **`references/`** holds supporting material linked from `SKILL.md`. Add scripts or assets when the workflow needs them.

## Add a skill

1. Create a top-level folder with a lowercase, hyphen-separated name, such as `review-java-code`.
2. Add a `SKILL.md` with YAML frontmatter containing `name` and `description`. Match the name to the folder. In the description, state what the skill does and give clues about when to use it.
3. Document the workflow in the body. Include the expected inputs, the deliverable, and how to handle missing information. Link to supporting files using relative paths.
4. Try the skill with a typical request and a request with incomplete inputs. Verify the output, file links, and any scripts it relies on.
5. Add the skill to the table above and open a pull request. Include an example prompt and a short note on what you tested.

Keep credentials, private learner records, and other personal data outside this public repository. Use synthetic data in examples.
