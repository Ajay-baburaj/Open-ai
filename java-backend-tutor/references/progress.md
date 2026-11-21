# Progress record and scoring

## Save and resume

Use a single durable Markdown record per learner and course, named Java_Backend_Tutor_Progress.md by default. Look for an explicitly associated progress file or a matching Library file before creating one. In a learner's existing durable project, use their designated record. Ask the learner to resolve multiple matching records if the correct course is unclear. Keep learner records out of the skill directory.

Read the latest version at session start. Update it after substantive submissions, interview answers, and scheduling changes so interrupted sessions can resume. In Work Mode, use the Library workflow to create or replace the record and retain its stable ID and write version. For a write conflict, reload and merge new evidence by session or question ID. If durable saving is unavailable, state that and output a portable checkpoint the learner can bring back. Confirm saved status only after a successful write.

## Record structure

- Profile: course name, experience, target role, minutes per session, study days per week, total study days, Java release, and optional start date or time zone.
- Plan: version, numbered study days with objectives, budget, exercise and evidence, weekly interview slots, capstone milestones, and deferred topics.
- Current position: next study day, pending prompt, attempt status, and next action.
- Competencies: topic, current status, latest evidence, date, and help used. Statuses are planned, introduced, practised with help, and demonstrated independently.
- Mistakes: topic, observed mistake, cause or tentative cause, corrective exercise, due study day, and independent retest result. Revisit after roughly one, three, and seven study sessions as useful. Shorten the interval if it recurs.
- Interview log: week, topics actually taught, questions, responses or concise evidence, whether assistance was given, rubric scores, and follow-up tasks.
- Capstone: link if available, completed milestones, runnable test evidence, and design decisions explained by the learner.

## Interview rubric

Score each assessed dimension from 0 to 3. Use unassessed when the interview did not elicit evidence.

| Score | Observable evidence |
| --- | --- |
| 0 | Attempt shows a major gap and cannot proceed |
| 1 | Partial answer or substantial prompting required |
| 2 | Independently meets the core task with minor gaps |
| 3 | Independently addresses requirements and relevant edge cases and tradeoffs |

Evaluate correctness against the contract, reasoning against the learner's explanation, testing against actual cases proposed or executed, and communication against the clarity of their explanation. Tie every score to an example. For final readiness, use independent evidence across coding, Java, Spring and SQL, design, and project communication. Flag dimensions below 2 or unassessed for targeted follow-up. A calendar milestone alone provides no assessment evidence.
