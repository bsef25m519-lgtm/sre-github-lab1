
## Functional Requirements
- *FR-01:* The system shall require full book details to be saved in the catalogue before any book copy can be issued.
- *FR-02:* The system shall verify the student's library card and account status on-screen prior to issuing any book, blocking expired, fined, or maxed-out accounts.
- *FR-03:* The system shall automatically calculate and apply a late return fine of Rs 10 per day following the 14-day loan period.

## Nonfunctional Requirements
- *NFR-01:* For up to 1,500 active member records and library catalogue searches, book lookup and availability queries shall execute in under 3 seconds on existing hardware.
- *NFR-02:* The web-based system interface shall allow the librarian or attendant to complete a standard book issue or return transaction in under one minute during peak rush periods.

## Acceptance Criteria
- *FR-01:* Given a book that is not yet in the catalogue, attempting to issue it fails until the complete book record and shelf location are saved.
- *FR-02:* When a student with an active fine or 3 currently issued books attempts to borrow another book, the system blocks the transaction and displays the restriction on screen.
- *FR-03:* When an overdue book is returned 3 days past the due date, the system automatically appends a fine of Rs 30 (Rs 10/day) to the student's account.

## Assumptions and Open Questions
- *Assumption A-01:* Student email addresses provided during registration are active and accessible via the university network.
- *Question Q-01:* What fallback procedure should be implemented if internet connectivity is temporarily lost during card verification?
- *Question Q-02:* Which administrative role holds final authorization for granting fine relief above 50%?

## Project Status and Viewing
- *Status:* Documentation and requirements specification phase. Full application implementation has not started.
- *Viewing:* Clone this repository and view README.md in a Markdown editor or inspect the rendered file on GitHub under the doc/feature branch.

## Author
- *Name:* Abdulrehman Khawaja (Roll No: 519)
- *Group Members:* Syed Ahsan Abbas (547), Ali Mehdi (555)
- *Course:* Software Requirements Engineering (PUCIT)

## Contributing
To propose changes to this documentation:
1. Create and switch to a documentation branch (doc/feature).
2. Edit and review the README.md file locally.
3. Stage and commit changes with a descriptive message.
4. Push the branch to remote GitHub (origin).
5. Open a pull request against the main branch for review.