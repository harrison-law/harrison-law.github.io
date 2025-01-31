---
layout: essay
type: essay
title: "To Ask or Not To Ask, That is the Question"
# All dates must be YYYY-MM-DD format!
date: 2025-01-30
published: true
labels:
  - Questions
  - StackOverflow
---

<img width="200px" class="rounded float-start pe-4" src="https://as1.ftcdn.net/jpg/03/16/75/44/1000_F_316754402_pZPt5WgtcCft285YG2p5vqkkPE2FlNqQ.jpg">

## Questions, questions, questions

In life, we all ask questions. Placed in this world with not a clue of what to do, we must ask questions in order to live and prosper as people. This same idea applies to software engineering, as no matter how smart we might think we are, we still need to ask questions sometimes. With this, we learn that the way we ask questions often times dictates the response we get, which can especially be true on various online forums such as StackOverflow. The homepage of programming questions galore, StackOverflow has become a site home to just about any programming question an aspiring software engineer might have, making it also home to various smart and less smart questions. But that begs the question: what makes a question... smart?

## Are some questions smarter than others?

Obviously the answer to this questions is yes (I guess this isn't the smartest question ever), but what makes that the case? To determine this, I went onto StackOverflow and looked for questions that I deemed as "smart" under the guidelines outlined by Eric Steven Raymond in "How To Ask Questions The Smart Way". After digging for a bit, one example of a "smart question" was regarding the difference between var functionName = function() {} versus function functionName() {} in Javascript, seen here.

```
Q: var functionName = function() {} vs function functionName() {}

I've recently started maintaining someone else's JavaScript code. I'm fixing bugs, adding features and also trying to tidy up the code and make it more consistent.

The previous developer used two ways of declaring functions and I can't work out if there is a reason behind it or not.

The two ways are:

var functionOne = function() {
    // Some code
};
And,

function functionTwo() {
    // Some code
}
What are the reasons for using these two different methods and what are the pros and cons of each? Is there anything that can be done with one method that can't be done with the other?
```

You can find the link to the forum [here](https://stackoverflow.com/questions/336859/var-functionname-function-vs-function-functionname). 

This question checks off many of the boxes of being a smart question, as it provides the reasoning behind the question, a direct and specific title, the programming language it is in, snippets of code to show exactly what is being asked, and open ended questions that provide room for thought and explanation that wouldn't be provided with just a Google search. Though I do have to take some points off for neither a "please" nor a "thank you", the question itself is a smart one, which is highlighted by the depth and conversation in response. This question garnered 42 responses, many of which provide an in depth explanation of the question at hand along with relevant examples and additional information, all of which contribute to a healthy and useful forum page. Through the question itself and the responses it received, I can confidently say that this was a pretty "smart" question that should have been asked.

## The flip side

To demonstrate that sadly not all questions can be deemed as smart, StackOverflow was once again scoured in search for a question that doesn't quite meet the criteria of a smart question. After my scouring, I stumbled upon this very quickly shut down question about the difference between structural and behavioral patterns, found here.

```
Q: Structural vs Behavioral Patterns. Need absolute clarity

Here I saw description for pattern types:

Structural - "Structural patterns are concerned with how classes and objects are composed to form larger structures."

Behavioral - "Behavior patterns are concerted with algorithms and the assignment of responsibilities between objects."

Can somebody explain the actual difference in plain simple English? Maybe a simple example.

```

You can find the link to the forum [here](https://stackoverflow.com/questions/79402043/structural-vs-behavioral-patterns-need-absolute-clarity).

This question doesn't quite accomplish the goals of a smart question, being that the question is vague and comes off as quite rude in wording. The question is also too open ended and can easily be seen as a time sink (as described in the above article), as these kinds of questions would lead to responses that can often be unhelpful or condescending. The example definitions themselves also don't contribute much to the question, as they are just thrown in without much explanation of what they want out of them. Once again I have to minus points for the lack of any "pleases" or "thank yous", which is just the cherry on top of poor attributes this question has.

## Conclusion

Though often people say that there are no such thing as dumb questions, some questions aren't worth asking without some further thought into how they are asked and what answer is wanted in response to the question. When asking questions in a public forum like StackOverflow, it is important that we as programmers with a question ensure that our question is worth people's time to answer, for both potential responders' sake and our own. Best of luck on your programming journey and I hope you make sure to ask those smart questions!
