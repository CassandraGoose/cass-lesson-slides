## Workflow: PR and GitHub Communication


Notes: 
have students keep open: https://frontend.turing.edu/lessons/module-2/workflow-prs-and-github-communication.html
---

### Goals
By the end of this lesson you will be able to...

- recognize what makes a README useful
- file and organize issues with labels and team member assignments
- explain and justify pull-requests and code reviews
- give professional and actionable feedback through code reviews

---

### Vocab: 

README, Project Board, User Story

---

### Warmup

https://frontend.turing.edu/lessons/module-2/workflow-prs-and-github-communication.html

notes: 
https://frontend.turing.edu/lessons/module-2/workflow-prs-and-github-communication.html

Give students: https://thejunkland.com/blog/how-to-write-good-readme.html

how you write readmes will change depending on where you work, what language, etc. 

---

What do READMEs have to do with PRs and github communication? 

It's all about good communication. You'll avoid a lot of back and forth, issues, etc that you'll encounter in PRs and GitHub communication when you have a good README.
<!-- .element: class="fragment" -->

---

Issues

GH issues are a great way to keep track of tasks, enhancements, and bugs for your projects. Project board trackers can often connect with GitHub issues and issues connect automatically with GitHub Projects.
<!-- .element: class="fragment" -->

Notes:

these issues don't usually include the HOW to do it.

React issues: https://github.com/facebook/react/issues
Vue issues: https://github.com/vuejs/vue/issues

demo Github Projects 
easy issue linking
trello -> https://blog.trello.com/github-and-trello-integrate-your-commits

---

Your Turn:

GH issues are often a great place to start when deciding what to work on, especially after you have setup a project board. Ideally, you should do this before you even start to code! Let’s get some practice!

---

Todo:
<style type="text/css" rel="stylesheet">
  .list {
    font-size: 22pt;
  }
</style>

<span class="list">

- Open up a project repo, click on the Issues tab, and then click the green New Issue button on the right.

- Think about a feature/bug that needs to be added. (Think of a specific small piece as opposed to a gigantic feature)

- Keep the title short and descriptive!

- Create a user story to determine what should happen. (Focus on the What, WHY, and WHO and less on the HOW)

- A good structure to follow with this is As a __, When I visit __, I want to __, so that I can __.

- Depending on the feature, you might even include Happy Path and Sad Path user stories!

- Think about any additional information that might be needed. This can included resources such as helpful links or relevant wireframes.
</span>

notes:
give examples of some user stories.

---

Breakout

- Let the other members read through your issue. The person sharing should NOT describe or fill in missing details.
<!-- .element: class="fragment" -->

- While reading through the issue, take notes of what parts are clear and what details are missing. (Reminder that the issue should not focus on the HOW)
<!-- .element: class="fragment" -->

- Share notes and actionable feedback with each other. Be prepared to share take-aways afterwards.
<!-- .element: class="fragment" -->

---

### Tags/Labels

Issue tagging with labels improves issue organization.
Multiple labels can be added to issues and allow for a developer to filter by one/many labels at once. This not only is helpful for the team but also for project managers to view what is being worked on and where a team is at.

---

![tags](https://assets-global.website-files.com/5ff621612284ed73d44c11f3/5ff621612284edbe0f4c1c58_5f19a241624e0709908d965b_robin-github-issue-tag-system.png)

Notes: 
 What kinds of labels are there? How might you combine these? What do you notice about the colors?

---
Add some labels to the issue you were just working on.

---

### Assignments and Linking

Assigning a person to an issue and linking an issue to a project board can again help in communication across the team on who is working on what at what time.

Notes: 
checkout the vue projects here and see how they are linked and assigned https://github.com/galio-org/galio/projects/4

---

Your turn:

- Assign yourself to your GH issue. (You should see your name next to the issue)
- Link the issue to your GH project. (You should now see the issue as a ticket on your project board!)
(These can be accessed on the right hand side of the issue near the Labels section.)

---

### Code Reviews and Pull Requests

Code reviews can be an enlightening part of the collaboration process. 

It can help identify technical issues that lead to improvements and can also identify areas for improvement regarding communication!

Notes: 
It _can_ be one of the only times that collaborative learning happens on teams that do not pair.

Can share your old teams system

A code review is often started with a PR.

---

A Pull Request (PR) is a method of submitting contributions to a project. 

Instead of pushing directly to a project, a PR acts as a medium for the members of a project to review the code and decide if it should be incorporated.

---

Post in the chat: 

What is a Pull Request?
<!-- .element: class="fragment" -->

What is the point of a Pull Request?
<!-- .element: class="fragment" -->

Notes:
benefits: shared fault, record of code and communication, filter to promote clean, bug-free (or as bug free as possible) code, place to ask questions and have discussions before time is wasted writing code that will not be used

---

Take a look at some examples of code reviews: 

https://frontend.turing.edu/lessons/module-2/workflow-prs-and-github-communication.html

notes:
talk about what is good and what is bad

---

##### Pull Requests

It is important as the creator of the PR that you are giving other developers some context of what they are reviewing as well as what they should looking for in the change. In order to standardize what is discussed, pull request templates were created. Follow the steps in the link to create one for your project. Here are some recommended questions to get you started:

```
#### What's this PR do?
#### Where should the reviewer start?
#### How should this be manually tested?
#### Any background context you want to provide?
#### What are the relevant tickets?
#### Screenshots (if appropriate)
#### Questions:
```

Notes:
find a link to read about how to create a pr tempalate in the lesson

---

GH Magic

- If you linked a PR to an issue, the issue will automagically close when the PR is merged 🎉

---

Checks for Understanding

- What are some benefits of using PRs and code reviews?
- What are some things that you can/should include in a README?
- Why are GitHub issues useful?
- What are PR templates useful?

Notes: 
- recognize what makes a README useful
- file and organize issues with labels and team member assignments
- explain and justify pull-requests and code reviews
- give professional and actionable feedback through code reviews

