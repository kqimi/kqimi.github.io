---
layout: essay
type: essay
title: "Design Patterns and the Recipe That Built Plate Mate"
# All dates must be YYYY-MM-DD format!
date: 2025-04-24
published: true
labels:
  - Software Engineering
---

When I first started coding in JavaScript, I approached it like a home cook with a pantry full of unfamiliar ingredients—excited, but often guessing. I could slice up an array or stir through an API, but my early projects lacked structure. The more complex they became, the more I found myself buried in spaghetti code. Then I discovered design patterns—and everything changed.

Design patterns are like the foundational recipes of software engineering: not specific to one language or framework, but rather reusable blueprints for solving recurring problems. Just as a chef doesn't invent lasagna every time they cook, a developer doesn’t need to reinvent architecture every time they build. With patterns, code becomes more readable, maintainable, and collaborative—qualities that are crucial now that I’m building Plate Mate, a group project designed to help students share their excess food on campus.

We’re using a Next.js template as the base for our project, and from the very beginning, I noticed how certain design patterns naturally fit into the workflow. For example, when managing how different components render user roles (admin vs. student), we turned to the Strategy Pattern. Instead of bloating our components with conditional logic, we abstracted role-specific behaviors into separate modules—letting the app stay flexible and readable as we add more roles and permissions.

Deploying our project with Vercel made it clear how important the Singleton Pattern is. We’re using Prisma for database access, and to avoid opening multiple connections during hot reloads or serverless executions, we implemented a singleton instance of the Prisma client. This simple yet powerful pattern stabilized our database layer—no more connection errors out of the blue.

Even managing state in React reminded me of design patterns. With multiple forms, modals, and data flows in Plate Mate, I’ve leaned on principles from the Observer Pattern to handle real-time UI updates. While we aren’t using a full-blown state management library, the ideas from this pattern help guide how components react to changes in shared data, especially when users post new food items.

I know that my experience with Bootstrap so far hasn’t been the best, but I understand why learning this type of framework is beneficial for job opportunities. Compared to raw CSS, Bootstrap has more limitations. For example, buttons in Bootstrap follow a standard look, and if you want a unique design, you’ll need to customize them using CSS.

At first, I didn’t realize I was using design patterns—I was just solving problems. But the more I code, the more I recognize them as part of a developer’s intuition, like muscle memory. Patterns aren’t rigid rules—they’re adaptable techniques that bring structure and clarity to complex systems.

So when someone asks me in an interview, “What are design patterns?” or “Which ones have you used?”—I think back to Plate Mate. To JavaScript and Next.js. To the way our team built a system that not only helps students reduce food waste, but does so with clean, scalable code behind the scenes. That’s the power of design patterns: they don’t just make software better—they make developers better too.


*ChatGPT was used to refine the grammar and the clarity of my writing, however, all ideas and contents are entirely my own.*
