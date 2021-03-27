# Code Reviews

In the Otrego, we believe in a culture of code-reviews for changes.

Code-reviews are a process to improve code-quality where another team member
takes a look at Changes (typically Pull Requests) and approves the changes. For
a detailed exploration of Code Reviews, we recommend the
[Google Guide on Code  Reviewing](https://google.github.io/eng-practices/review/).

## Process

**Overall** The goal with Code Review is to ensure that the code in the change
is generally consistent with Otrego best-practices. The goal is *not to ensure
perfection*. Even if you, as a code-reviewer, have *no comments* just having a
second pair of eyes on code tends to improve code-quality.

2.  **Code Reviews should be Quick**. Code reviewers should respond to the code
    review in ~24 hours and aim to complete the code review in 2-3 days or
    less, depending on the size of the code reveew. If a code-reviewer hasn't
    responded on a Pull Request in 24 hours, it's OK to ping the code-reviewer.

1.  **Focus on Understanding** Focus on understanding the change first. What is
    the Pull Request trying to do? Feel free to ask questions! Otrego is about
    collaboration and part of collaboration is the learning that happens during
    Code Review.

2.  **Make Suggestions** Go through each of the files in the Pull Request, making
    [suggestions and comments](https://google.github.io/eng-practices/review/).

  *   *Design*: Is the code well-designed?
  *   *Functionality*: Does the code behave as the author likely intended? Is
      the way the code behaves good for its users?
  *   *Complexity*: Could the code be made simpler? Would another developer be
      able to easily understand and use this code when they come across it in
      the future?
  *   *Tests*: Does the code have correct and well-designed automated tests?
  *   *Naming*: Did the developer choose clear names for variables, classes,
      methods, etc.?
  *   *Comments*: Are the comments clear and useful?
  *   *Style*: Does the code follow our style guides?j
  *   *Documentation*: Did the developer also update relevant documentation?


3.  **Resolve suggestions and comments** If you you make comments/suggestions
    and you *don't approve* the pull request, the expectation is that the code
    review author needs to fix the suggestions before approval can be achieved.
    As code reviewer, you should make it make it clear to the author which
    comments are non-blocking. For example, we usually prefix minor changes
    with "nit: ".

4.  **Approve & Merge the Pull Request!**
