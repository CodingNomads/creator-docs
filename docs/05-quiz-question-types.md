# Quiz Questions

Quiz questions are primarily meant as a chance for students to become active in their learning process, after having read or watched some content passively. They serve as quick check-in points and don't need to be too complex. Keep the questions and question types simple, both for your own and your students benefit. The main value of quizzes are:

- **Activate**: Switching from passive to active learning
- **Double-Check**: Self-check-in for students whether they understood the main concepts from a section

This is why we suggest to use **multiple-choice** or **true/false** questions. We have experimented with using other question types of the many that our learning platform offers, but keeping it simple has proven to be the best way to go in terms of quizzes.

## Importing Quiz Questions

Moodle supports a text format called `.gift` for importing quiz questions. The format is human-readable, which makes it a good option to create your quiz questions alongside your Markdown content, and keep them version-controlled, but be able to quickly add them to your course on the platform.

The screencast below walks you over how to create questions in this format and upload them to the platform:

<iframe width="560" height="315" src="https://www.youtube.com/embed/Zdrdh_Y7HWo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

To learn more, read over this concise <a href='http://buypct.com/gift_reference.pdf' target='_blank'>GIFT Reference sheet</a>, or download it from the <a href='https://drive.google.com/drive/folders/1m6jfPz803rZMDp1vLDKQz72nCLzek_UA' target='_blank'>Resources Folder</a>.

Here are two example questions written in `.gift` format, the first one being a multiple-choice question, the second one a True/False one:

```text
Do you like this format? {
    ~no
    ~maybe
    =YESSSS!
}

Uploading quiz questions saves some of your valuable time {TRUE}
```

Check out the screencast and the linked reference sheet to learn about additional options, such as question feedback, answer percentages, question names, and automatically adding questions to categories.

If you want to create your questions directly on the platform instead of going down the `.gift` route, keep reading below for some information to keep in mind.

---

## Multiple Choice and Single Choice Questions

Choose the appropriate type when creating a question. Make sure that the following settings are applied:

- **Adaptive Mode**: Grading should be set to _Adaptive Mode_ to allow students to check whether they have the correct answer or not. Quizzes are meant as a learning experience, not as a test
- **No Penalties**: Make sure that penalties for wrong answers are set to `0`. Again, quizzes are for learning and you don't want to penalized students for getting it wrong
- **Percentages**: You will have to assign a percentage of the total point score to each answer. Make sure that these add up to 100%. E.g. if you are creating a true/false question, the correct answer should get `100%` and the wrong answer should get `0%`. If you are creating a multiple choice question, the percentages of all correct answers should add up to `100%`. If there are 3 correct answers, choose the `33.33%` setting for each of them

As mentioned above, attempt to keep the quizzes simple. Most of the time using these two question types will be enough to give your students the experience of switching into a simple active learning mode, and helping them to check up on how much they were paying attention in the previous section.

## Code Runner Questions

Code Runner questions allow your students to write and execute code snippets, to test their practical understanding and train their coding skills. The screencast below explains how to set up a Code Runner question for your Quiz resource:

<iframe width="560" height="315" src="https://www.youtube.com/embed/1wMXtM0RSxs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Feedback Resource

The Feedback Resource is not exactly a quiz, but it prompts students to answer questions as well. It is a _different resource type_ that has a specific template we want you to use. After creating the Feedback resource, you can select the template in the "Templates" tab:

<iframe width="560" height="315" src="https://www.youtube.com/embed/IBOKVGzO534" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
