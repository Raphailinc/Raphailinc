# Public project guide

[Profile](README.md) · [Русский](PROJECTS.ru.md) · [Engineering case studies](case-studies/README.md)

For a Python backend review, start with the six pinned repositories. Try the [infrastructure-free campaign demo](https://github.com/Raphailinc/Task-Delay-Service#try-the-complete-flow-without-infrastructure), then read the [delivery design](https://github.com/Raphailinc/Task-Delay-Service/blob/main/docs/delivery-design.md). The remaining active projects explore specific tools, languages and algorithms.

## Python backend and libraries

| Repository | A useful path through the code |
| :--- | :--- |
| [altpkg-diff](https://github.com/Raphailinc/altpkg-diff) | Follow the HTTP client into package comparison and the CLI. The [HTTP contract tests](https://github.com/Raphailinc/altpkg-diff/blob/main/tests/test_api_contract.py) cover bounded retries, malformed upstream responses and resource cleanup. |
| [Task Delay Service](https://github.com/Raphailinc/Task-Delay-Service) | Follow campaign validation into recipient selection, local time windows and Celery jobs. [Scheduling regressions](https://github.com/Raphailinc/Task-Delay-Service/blob/main/api/tests/test_scheduling_regressions.py) cover midnight boundaries and invalid audience filters. |
| [Pulse](https://github.com/Raphailinc/Pulse) | Explore the Flask factory, content ownership and shared image validation. [Upload tests](https://github.com/Raphailinc/Pulse/blob/main/tests/test_uploads.py) exercise invalid content, pixel limits and file replacement. |
| [Car API](https://github.com/Raphailinc/Car-API) | Inspect Marshmallow schemas and transactional CRUD handling. [API tests](https://github.com/Raphailinc/Car-API/blob/main/tests/test_api.py) cover VIN uniqueness, invalid domain values and updates. |
| [Taskboard](https://github.com/Raphailinc/Taskboard) | Trace Django forms, owner-scoped queries and protected downloads. [Attachment tests](https://github.com/Raphailinc/Taskboard/blob/main/myapp/tasks/test_attachments.py) cover cross-account access, CSRF and deletion methods. |
| [Document Detector](https://github.com/Raphailinc/Document-Detector) | Read contour detection and perspective transforms, then the [synthetic-image tests](https://github.com/Raphailinc/Document-Detector/blob/main/tests/test_detector.py). |

## Data and numerical experiments

| Repository | Focus |
| :--- | :--- |
| [Country Parser Toolkit](https://github.com/Raphailinc/Country-Parser-Toolkit) | Offline HTML parsing tests, normalized country records and summary statistics. |
| [Monte Carlo](https://github.com/Raphailinc/Monte-Carlo) | Seeded integration estimates, variance and standard error. |
| [Random Sequence Analysis Toolkit](https://github.com/Raphailinc/Random-Sequence-Analysis-Toolkit) | Distribution summaries, observed repeats and chi-square statistics. |
| [Random Variable Distribution Toolkit](https://github.com/Raphailinc/Random-Variable-Distribution-Toolkit) | Inverse transformation sampling and theoretical bin probabilities. |
| [Text Analyser CLI](https://github.com/Raphailinc/text-analyser-cli) | Image preprocessing and an OCR interface tested with a stub. |
| [Big Data Lab](https://github.com/Raphailinc/Big-Data-Lab) | Scala CLI, in-memory statistics and unit tests. |

## Web applications and collection tools

| Repository | Focus |
| :--- | :--- |
| [Mars Lab Project](https://github.com/Raphailinc/Mars-Lab-Project) | Express/MongoDB report submission and React forms. |
| [Micro Video Hosting](https://github.com/Raphailinc/Micro-Video-Hosting) | SvelteKit, SQLite, video uploads and tags. |
| [vprok parser test task](https://github.com/Raphailinc/vprok-parser-test-task) | Separate browser and API collection approaches. Live runs depend on the upstream site. |

## Other languages

| Repository | Focus |
| :--- | :--- |
| [ToolOps](https://github.com/Raphailinc/ToolOps) | C++17 domain model, TSV persistence and tests. |
| [Dice Duel](https://github.com/Raphailinc/Dice-Duel) | C++17 game rules, seeded simulation and tests. |
| [ToDo CLI](https://github.com/Raphailinc/ToDo-CLI) | Java 17 task repository, SQLite and JUnit. |

## Archived learning projects

These early browser and PHP exercises are preserved as read-only learning history. They are separate from the active backend portfolio.

| Repository | Focus |
| :--- | :--- |
| [Product Atlas](https://github.com/Raphailinc/Product-Atlas) | PHP JSON endpoints, a product catalog and reviews. |
| [2D Net](https://github.com/Raphailinc/2D-Net) | Rubik's Cube move visualization. |
| [Biomorph Playground](https://github.com/Raphailinc/Biomorph-Playground) | Generative forms and reproducible genomes. |
| [Dragon Curve Playground](https://github.com/Raphailinc/Dragon-Curve-Playground) | Recursive geometry and SVG export. |
| [RealCross](https://github.com/Raphailinc/RealCross) | A static responsive website. |

These repositories are portfolio and learning projects. Each README explains setup, checks and operating scope. Commercial experience and personal implementation case studies are described in the [profile](README.md).
