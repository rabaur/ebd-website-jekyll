# Adding/Editing a Lecture Item
The site displays a list of all lectures in the semester. Each lecture item is generated from a `.md` file in `./_lectures`, e.g. `./_lecturers/lecture1.md`. In each of these files, you will find the following _front matter_:
```
---
date: 2024-09-18 18:00:00
topic: Introductory Lecture
lecturers: [Minerva McGonagall, Severus Snape]
type: lecture
recording:
slides:
---
```
The front matter is used to set the information about the lecture:
- `date`: The start date of the lecture in the format `YYYY-MM-DD HH:mm:SS`.
- `topic`: A short description of the lecture topic
- `lecturers`: A list of lecturers, surrounded by square brackets and delimited by commas.
- `type`: A categorization of the lecture, e.g. `talk`, `lecture`, `tutorial`, ...
- `recording`: The link to the recording. Make sure to create a password protected link.
- `slides`: The link to the slides. Make sure to created a password protected link.

