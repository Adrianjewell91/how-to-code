For the Lay Audience: How Computer Programmers Think 

*Introduction (Know)*

There is no doubt that software engineers are in high demand. As a case in point, the website LinkedIn.com, posted 335,000 software engineer jobs last weekend in the United States. But despite the abundance of excellent online curriculum that is freely available, it is not easy to learn to code. One reason, among many, is that it is hard to pick the right curriculum. How can somebody trust that their curriculum is trustworthy? There isn’t a clear answer.
In fact, today on the internet, there are a lot of courses about how to code. On Udemy, there are 10000 results given a search for “coding.” On Google, a search for “learn to code” will return 7,020,000,000 results. These numbers show that there is a lot of information for a student of coding. Even for an eager student, it would take too long to sift through this library of knowledge. 
This course is the solution to this problem. I am a software engineer with several years of experience, and I wrote this course to give students the most important knowledge for learning to do software engineering. Personally, I got into coding through a bootcamp, then I worked in the industry, and also worked full time as a coding instructor. During this time, I learned something very valuable:

    If you learn to think correctly, you can teach yourself anything that is programming-related very easily.

The truth is: the majority of online coursework teaches you very specific skills, but it doesn’t teach you how to think correctly. Just do a search on Google. You will see that all courses have titles like: 
“Intro to Python”,
“Intro to Machine Learning”, 
“Working with Kubernetes”, 
“Build a Javascript Web Application in seven days”. 
While these courses are useful, they only teach a specific programming skill. If you study the information in this book, then you will be able to learn any of the skills mentioned above, and more, in a very short time, without any hand-holding that usually happens in courses. That will make you very powerful. 

*The Process:*

The fundamental skill is software engineering is learning how to thinking about problems in terms of inputs and outputs:

    INPUTS -> OUTPUTS

This may sound simplistic or contrived, or perhaps obvious, but actually it is not. To exemplify, let’s say that you want to build an App for your phone that lets you read emails. If you want to build an application like this, you will probably be thinking in your mind, something like this: 
    As a user, I want to go on the app and view my emails.  
Now, this makes sense. This particular sentence isn’t actually saying anything different that what we originally said in the previous paragraph, but let’s think about this for a minute. Actually, there are some other things that are also probably true about this phone app, such as :

    As a user, I want to go on the app and see my emails, and NOT OTHER PEOPLE’S. 

This may be self evident, from the previous statement, but it’s actually not. If somebody asked me to build that app for them, and they told me the first statement, I’d ask them, “Do you want to only see your own emails, or do you want to see your emails along with other peoples emails?” This is a valid question because the former statement doesn’t specify, while the latter statement does make this clarification. You might think this is a contrived example, but the only reason why you think this is because in today’s world, when we talk about viewing email, we automatically assume we only want to see our emails. This kind of thinking, however, is jumping to conclusions, and that’s something we want to avoid in software engineering. 

Now, another thing that is probably true about your app is this:

    As a user, I DO NOT want other people to be able to view my emails.  

This might also be implied by the original statement, but it’s really not. Once again, in today’s world, people generally assume that emails are private and confidential, but it’s very possible that this particular App does not treat emails as confidential information. Therefore, we must once again clarify. 

At this point, it is possible to see that this kind of clarification of requirements could go on further, perhaps with something like this:

    As a user, I want to view my emails…
            FROM ANYWHERE IN THE WORLD,
            AND THEY SHOULD LOAD QUICKLY,
            AND ANY EMAIL I RECEIVE SHOULD NOT BE CHANGEABLE AFTER I RECEIVE IT.

And this does happen in the real world. In fact, all of these additional requirements are very interesting and challenging software problems that engineers have worked on for years. For now, however, we will not tackle these additional things. In fact, this process of question clarification is not even the key skill in software engineer (rather, it’s simply critical thinking), but a software engineer must engage in this line of inquiry for sake of arriving at an answer to the original goal: how to view a problem in terms of inputs and outputs. In the case of this example:

    INPUTS (Username and Password) -> OUTPUTS (The Emails associated with the Username)

The reader should now see how the original line of inquiry led the software engineer to decide on these inputs and outputs. In case they are not clear, a brief explanation is as follows. The engineer chose the username and password because these are unique identifiers to the user. That is, they identify the user in such a way that every user is distinguishable from every other user. In this way, the App can filter for only the emails associated with the user and exclude the others. The password, similarly, is the way that the user verifies that the user is in fact the user. In this way, only a user him/herself can view the emails associated with them. Having explained this, it is possible to see how the choice of a username and password is at least one possible way to fulfill the requirements. 

This is a very interesting example, for several reasons. Firstly, it is interesting because the reader can see how even something as simple as an email application can require some concerted thinking. Secondly, it is the author’s hope to give a lay reader some insight into software applications that an average person probably uses multiple times a day.  Thirdly, the reader can see how something as commonplace as logging-in is something about which engineers seriously reasoned.  Mostly, importantly, however, this introduction to problem solving demonstrations the first of a series of steps, which we will call: 

    1. CLARIFY THE PROBLEM

Clarifying the problem is the first of five steps in a problem solving process that any programmer will go through when they write a computer program.  The remaining steps are as follows:

    1. WRITE TEST CASES
    2. BRAINSTORM STRATEGIES
    3. PICK A STRATEGY
    4. WRITE PSEUDO-CODE
    5. WRITE CODE
    6. VERIFY/TEST (ACTUALLY IS DONE THROUGHOUT THE WHOLE PROCESS)

It will take a little bit of time to explain this process, but rest assured that if you master this process, you can become a software engineer.  You may have noticed that this list begins with “1. WRITE TEST CASES”. Isn’t “CLARIFY THE PROBLEM” the first step? In actuality, these steps are one and same, but under slightly different names. Continuing with our example will illustrate this point. Consider that the engineer building the web app has arrived at the decision from before: where user inputs a username and password, and the user’s emails are returned to the user. Is this enough information to begin writing a computer program?

If you thought the answer is “yes”, then you are clearly a very thorough thinker, because that would mean that you had already come up with answers to a variety of questions that must be answered before any programmer can build this app. Some of these are:

    What is a valid username?
    What is a valid password?

    What happens when invalid credentials are entered?
    What happens when empty credentials are entered?

    How many of the users emails do we want to return? 

In fact, a computer programmer must answer these question before building the application. Why is that? Well, it’s because there is more than one answer to these question. Certainly, the engineer must decide what to do, and there may be even more questions worth asking and answering. Given the fact of the matter, one might notice that these questions are slightly more specific than the original questions we were asking earlier. Therefore, they might fall under the category of “TEST CASES” rather than “CLARIFYING THE QUESTION,” but in actuality, they are very closely related to one another. Writing these tests cases is extremely important, perhaps the most important part of computer programming, and later on this in this course, we will dive deeper into strategies that ensure you have met all test cases for a problem. 

At this point, it is my hope that this example has made you interested in the process of software engineering. You may also notice that we haven’t done any coding yet.  That is intentional, because my goal is to teach you the process of computer programming, and computer programming actually starts with this process of trying to understand the problem as clearly as possible. Once the programmer understands the problem, then he or she will begin steps two through six, which are more related to coding.  In the remaining portion of this introduction, I will walk through the remaining steps, but in order to do, I will switch gears a little bit. 

To illustrate the remaining five steps. We are going to use a different example for the sake of clarity.  While it is true that we could continue explaining the steps using the example of the Email Application, the truth of the matter is that building an email application requires a lot of specific technical knowledge that will hinder more than help in my explanation of the problem solving process. Believe it or not, the problem can actually be a very vast one, so for the purposes of this course, and the remainder of this introduction, we are going to tackle a simple problem instead.

The problem I’d like to tackle is that of deciding whether two numbers add up to a third number. This may sound like an astonishingly simple task, but that is a good thing, because it will allow us to concentrate solely on the problem-solving process. Now, let us recall that the goal of the engineer is to transform the problem into a series of inputs and outputs:

    INPUTS -> OUTPUTS

In this case, there aren’t too many clarifying questions that need to be answered. Probably, we can assume that numbers are real numbers. They can be positive or negative, or zero. We can assume the addition operator works as we normally expect it to work. So these are some assuring assumptions. Now, we must accomplish the task, and probably we would arrive at something like this:

    Three numbers (a, b, c) -> True or False

This should make sense. We have two numbers, and we want to know if they add up to the third number, and so the answer we want is either a “Yes” (True) or “No” (False). 

Now, to prove that we understand this, we must write some test cases that demonstrate our command of the problem, for example this one:

    1,2,3 => True 

We know this to be true because one plus two equals three. Here is another one:

    3,4,10 => False 

And a few more:

    -3, 0, 3 => False 
    -4, -4, -8 => True

This seems like a relatively straightforward and maybe redundant practice, but it is actually very important this reason: sometimes we don’t know how to get the outputs from the inputs. This can happen for several reasons, and if you continue with the course, you will learn about those situations, and what to do about them. But in all cases, what engineers need to do is come up with more test cases. In the first part of this course, we will cover strategies that make sure you come up with all possible test cases. For the time being, we can be satisfied with the above test cases. 

The next step is to brainstorm strategies. Maybe, in your mind, there is only one strategy, but to an engineer, there is always more than one way to do something. Here are a few ideas:

    1. Add the two numbers together, and compare the sum with the third number.

This is one way to do it, but here is another way.

    2. Subtract the second number from the third number, and compare it with the first number	

This solution is equally valid. Some of you might think these two solutions are the same. Fundamentally, they accomplish the same thing, but they are not the same solution because they are doing different mathematical operations, and this might be an important detail for an engineer. We will see why when we get further down in the process. Lastly, it is important to note that while this problem had two very obvious solutions, there might certainly be more solutions. The corresponding chapter in this course will cover strategies to come up with the solutions when no solutions come to mind. The technique for doing this are perhaps the most powerful techniques you can learn from this course, and it is still a field that I personally feel is an area for significant academic research. 

In practice, coming up with solutions can be hard because requires the engineer to introspect into their mind and be able to express, in words, how the inputs were transformed into the outputs. There are many strategies to help with this process, and they are outlined and the end of the chapter. This step is the most important, and it is both a creative and disciplinary process - the former because insight is required, and the latter because attention to detail is required to put that insight completely into words. 

For now, we can be satisfied with these two solutions. The next step in the process is to pick one of them. In order to accomplish this, we must weigh the trade offs of each solution. When evaluating solutions, there will usually be pros and cons of each, and software, there will usually be a trade off in terms of how quickly the solution will run. This is common metric because people care about fast their computer programs run. In this particular case, it is very possible that one of these solutions will run faster than the other because of the mathematical operations being performed. That is, sometimes an addition operation will happen faster than a subtraction operation on a computer. This may a trivial performance increase on a modern machine, but imagine a hypothetical scenario from a time in the past, where the difference would be significant. In that case, there is a very good reason to pick one solution over the other. All in all, it is simply enough to know that this kind of weighing takes place in the problem solving process, and it’s important to know what the tradeoffs might be when picking a solution.

We will pick the first solution, and at this point, we come to the fourth steps: that of writing pseudo code. Finally, a step involving the word “code” - but only pseudo-code. That is, code that is not really code, but more of an in-between of English and the high level programming languages we know of today, such as Python, Javascript, Ruby, Java, etc. For our solution, we would probably describe it with the following:

    1. numbers a, b, c
    2. d = a + b 
    4. return d == c

In line one, we recognize that we have three numbers. In line two, we get the sum of the numbers, and in line three, we give the answer. This is pseudo because it looks like code, but isn’t formal syntax of a particular programming language.  In other words, it’s basically code if we could be ultra lazy in the way we wrote code. At this point, it’s fair to say that the engineer probably needs be at least familiar with coding to write the above statement. They should probably have taken a codeAcademy course on a programming language of their choice in order to be familiar with this kind of writing. But this shouldn’t be too hard to do, because that will take approx. 30 hrs or so, and then you will have learned how any major programming language is written. At that point, it won’t be hard to write pseudo-code. At the same time, getting to writing peusdo can actually be one of the hardest things to do throughout this process, and we will tackle strategies for writing later on. 

Lastly, one must turn the pseudo code into real code. In order to do this, one must actually know how to code, and having some fluency with the language syntax and knowledge of running code will be required to run the program.  For a student, they might write something like this:

    function TwoNumbersAddToThird(a, b, c) {
        return (a + b) === c;
    }   

This is an implementation of the function in the programming language javascript. Even without any formal study in programming languages, the average reader can probably grasp how this function works, and how it relates to the peusdo-code above. If that is the case, then the read should be encouraged by this new ability they have discovered.  However, if the connection was not apparent, then it would be important for you take a CodeAcademy course on Python or Javascript, or another language of your choice to get a grip on basic syntax before you dive any deeper into this course. It will not be important for the student to be skilled at programming to appreciate this course, but it will be necessary for the student to understand the foundations of how to write code. At very least, the student should be able to see how this function is derived from the pseudo-code above. Later on in the course, we will see that the process of translating pseudo code into real code can still be a very arduous process, requiring hours of research into programming languages, or understanding the machine that will ultimately run the code. 

Despite this, however, go from pseudo-code is really the very easiest out of all the six steps because the main skill required is grit rather than creativity and insight, but grit is not be undervalued. In fact, it is common knowledge that the most important factor in success is discipline and perseverance. In this final step, this kind perseverance is what allows somebody to do what we call “DEBUG” the code: the process of writing code, having the code churn out the wrong answer, then figuring out why it failed and trying to fix it. This is a skill that takes time to develop, and we will give tips for working on this too. 

If you test your code, and it works. Then congrats! You solve a problem. It is recommended to solve 150 of these problems (Go onto either Codesignal.com or Leetcode.com). If you do that, and keep practicing until you can solve medium level problems within forty-five minutes, then consider yourself a skilled coder, and apply for a job as a software engineer. Of course, that number is a rough estimate, taken from the amount of LeetCode.com problems that the company Google thinks an aspiring engineer should solve before one is ready to interview. 

Some reader say think that the information presented thus far is common knowledge, or widely available already. That is all true, but that is precisely why this content is part of the course’s the introduction. Rather, the aim of the actual course is to technique cognitive techniques and theory that will allow the engineer to effortlessly do the process, and do it well. 

*An Exercise: (WANT TO KNOW)*

Think of a problem you have yourself in your life and want to solve, and go through this problem solving process. Can you think of the problem in terms of inputs and outputs? Where do you get stuck in the process? What gets you unstuck? Write all of this down on paper and reflect on it in a journal entry. Answer these questions and gives examples to yourself. It could be any kind of problem, anything at all. 

*Strategies: (LEARNED)*

Strategies that help with the various stages in the problem solving process:

1. Clarifying the problem and generating test cases: 
    - Put yourself in lots of situations where people point out a test case that you hadn’t thought of yourself, and you feel embarrassed that you didn’t think of that yourself. Then you will remember to think "outside the box" next time.
    - Question the assumptions you are making about the problem.
2. Coming up with strategies:
    - Think of more test cases and observe how they are similar. Then use these similarities to explan how you get from the inputs to the outputs. If you can't visualize the steps or explain them, then do simpler test cases and gradually get more complex. 
    - Write it out: Write out the steps that your mind takes in English. Write it all down. 
    - Draw Pictures (Why is bubble sort called bubble sort?)
    - Subdivide the problem: If you can get "halfway" to the answer, then that is a good start. Try to break the problem into smaller and smaller chunks. 
    - If you have an idea, no matter how vague or wierd: Flesh it out and explore the idea to see what happens. 
3. Pick a solution: Be evaluated on your judgement many times over and over again. Learn about Time and Space Complexity.
4. Pseudo-Code: Lots of coding and reading solutions.
5. Code and Test: Lots of coding and reading solutions. 
    - Take a Programming Langauge Course on Codecademy.com.
    - If your code doesn't work, debug the code by putting print statements at various places in the code to see the state of the program at that moment in time.
    - If you're reading a solution and you don't understand it, do the code out on paper. Do not take shortcuts. "Doing the code" means stepping through the code, line by line, tracking all the variables. If you do this, you will understand the code, and you will gain insight.
    - Study everything about the machine that will run the program. In todays era, that machine is the personal computer. Understanding the machine that run your program will make it easier for you to program them.
6. Always be testing your ideas along the way. Do you have an idea? Test it with a new test case.

Profound statements: 
1. We have ideas before we understand them. That is, when you have an idea, you actually must explore it and try it out before you know what you actually comprehend what you meant. 	
2. We often cannot run understand code by reading it. We must run the code or do it out by hand. 
3. Probably, you don't understand the code you wrote, you must do the code to understand it.



