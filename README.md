# For the Lay Audience: How Computer Programmers Think 

*Introduction (Know)*

There is no doubt that software engineers are in high demand. As a case in point, the website LinkedIn.com, posted 335,000 software engineer jobs last weekend in the United States. But despite the abundance of excellent online curriculum that is freely available, it is not easy to learn to code. One reason, among many, is that it is hard to pick the right curriculum. How can somebody trust that their curriculum is trustworthy? There just isn’t a clear answer.

In fact, today on the internet, there are a lot of courses about how to code. On Udemy, there are 10000 results given a search for “coding.” On Google, a search for “learn to code” will return 7,020,000,000 results. These numbers show that there is a lot of information for a student of coding. Even for an eager student, it would take too long to sift through this library of knowledge. 
This course is the solution to this problem. I am a software engineer with several years of experience, and I wrote this course to give students the most important knowledge for learning to do software engineering. Personally, I got into coding through a bootcamp, then I worked in the industry, and also worked full time as a coding instructor. During this time, I learned something very valuable:

    Learning to think correctly will allow the student to easily teach him/herself anything programming-related.

The truth is: the majority of online coursework teaches you very specific skills, but it doesn’t teach you how to think correctly. Just do a search on Google. You will see that all courses have titles like: 
“Intro to Python”,
“Intro to Machine Learning”, 
“Working with Kubernetes”, 
“Build a Javascript Web Application in seven days”. 
While these courses are useful, they only teach a specific programming skill. Instead, if you study the information in this book, you will be able to learn any of the skills mentioned above, and more, in a very short time, without any hand-holding that usually happens in courses. That will make you very powerful. 

*The Process:*

The fundamental skill is software engineering is thinking about problems in terms of inputs and outputs:

    INPUTS -> OUTPUTS

This may sound simplistic or contrived, but actually it is not. To exemplify, let’s say that you want to build an app for your phone that lets you read emails. If you want to build this application, you will probably be envisioning yourself using the app, in a scenario such as this:

    As a user, I want to go on the app and view my emails.  
    
Such an expression is how the software engineer thinks about that particular idea in his or her mind.  In actuality, this particular sentence isn’t actually saying anything different that what we originally said in the previous paragraph, but it additionally implies a greater degree of specificity thereof. Let’s think about this for a minute. 

In other words, there are some other things that are also probably true about this phone app, such as:

    As a user, I want to go on the app and see my emails, and NOT OTHER PEOPLE’S. 

That little addendum at the end may have shocked a few people to respond like this: "Duh!", but do not be so quick to react in that way. If somebody asked me to build that app for them, and they told me the first idea:

    As a user, I want to go on the app and view my emails.

I’d ask them, “Do you want to only see your own emails, or do you want to see your emails along with other peoples emails?” Really, this is a valid question because this statement doesn’t specify, while the addendum in capital letters in fact makes this clarification. You might think this is a contrived example, but the only reason for thinking that is because: in today’s world, when people talk about viewing email, they automatically assume they only want to see their own personal emails. This kind of thinking, however, is jumping to conclusions, and that’s something to always avoid in software engineering. 

Now, another thing that is probably true about the mail app is this:

    As a user, I DO NOT want other people to be able to view my emails.  

This requirement might also be implied by the original statement, but it is actually not implied at all. Once again, in today’s world, people generally assume that emails are private and confidential, but it is very possible that this particular app does not treat emails as confidential information.

Now at this point, it is possible to see that clarification of requirements could go on further, perhaps in a way like this:

    As a user, I want to view my emails…
            FROM ANYWHERE IN THE WORLD,
            AND THEY SHOULD LOAD QUICKLY,
            AND ANY EMAIL I RECEIVE SHOULD NOT BE CHANGEABLE AFTER I RECEIVE IT.

Most people would expect this level of reliability from their email app. In fact, all of these mentioned requirements are very interesting and challenging software problems that engineers have worked on for many years. But that is besides the point. For now simply understand the clarifying requirements is a major part of a software engineer's initial look at a problem must begin. In fact, this process of question clarification is not even the key skill in software engineer (rather, it’s simply critical thinking), but a software engineer must engage in this line of inquiry for sake of arriving at an answer to the original task, which was: how to view a problem in terms of inputs and outputs. In the case of this example, the answer is as follows:

    (Username and Password) -> (The Emails associated with the Username)

The reader should now see how the original line of inquiry led the software engineer to decide on these inputs and outputs. In case they are not clear, a brief explanation is as follows: The engineer chose the username because this is an "unique identifiers" to the user. That is, the username can identify the user in such a way that every user is distinguishable from every other user. Using this information, the app can then filter for only the emails associated with the user while excluding the others. The password, similarly, is the way that the application verifies that the user is in fact who they say they are. In this way, only a user him/herself can view the emails associated therewith. Having explained this, it is possible to see how the choice of a username and password is at least one possible way to fulfill the requirements settled upone earlier in the discussion,
    
    - As a user, I want to go on the app and see my emails, and NOT OTHER PEOPLE’S.
    - As a user, I DO NOT want other people to be able to view my emails.  

This is a very interesting example, for several reasons. Firstly, it is interesting because the reader can see how even something as simple as an email application can require some concerted planning and clarafication. Secondly, it is the author’s hope to give a lay reader some insight into software applications that an average person probably uses multiple times a day.  Thirdly, the reader can see how something as commonplace as the login screen is something about which engineers seriously thought over. 

The name of what just happened above is called:

    1. CLARIFY THE PROBLEM

Clarifying the problem is the first of six steps in a problem solving process that any programmer will do when they write a computer program.  The remaining steps are as follows:

    1. WRITE TEST CASES
    2. BRAINSTORM STRATEGIES
    3. PICK A STRATEGY
    4. WRITE PSEUDO-CODE
    5. WRITE CODE
    6. VERIFY/TEST (ACTUALLY IS DONE THROUGHOUT THE WHOLE PROCESS)

It will take a little bit of time to explain this process, but rest assured that if you master this process, you can do software engineering. Now, you may have noticed that both “WRITE TEST CASES” and “CLARIFY THE PROBLEM” claim to be part of the first step. That is actually correct because these steps are one and same, but with slightly different names. 

Continuing with the example of the email application example will illustrate this point. Consider that the engineer building the web app has arrived here:

    (Username and Password) -> (The Emails associated with the Username)
    
Is this enough information to begin writing a computer program?

The answer is no, because more questions must be answered before any programmer can build this app. Some of these are:


    What is a valid username?
    What is a valid password?

    What happens when invalid credentials are entered?
    What happens when empty credentials are entered?

    How many of the users emails do we want to return? 

A computer programmer must also answer these questions before building the application. Why is that? Well, it’s because these questions have more than one answer. Thus, the engineer must decide the answer, and there may be more questions worth asking and answering. Given the fact of the matter, one might notice that these questions are slightly more specific than the first questions that were asked earlier. Therefore, they fall under the category of “TEST CASES” rather than “CLARIFYING THE QUESTION,” but as iterated before: both categories are very closely related to each other. Writing these tests cases is extremely important, perhaps the most important part of computer programming, and later on this in this course, the reader will find an outline of strategies to ensure the finding of all test cases for a problem. 

At this point, it is my hope that this introduction has made the reader interested in the process of software engineering. The reader also may also notice that the problem solver hasn't done any coding yet.  That is intentional, because this text's goal is to teach the process of computer programming, and computer programming actually starts with this process of trying to understand the problem as clearly as possible. Once the programmer understands the problem, then he or she will begin steps  more related to coding: two through six. The remaining portion of this introduction with walk through the remaining steps, but in order to do necessitates the switching gears (a little bit). 

To illustrate the remaining five steps, a different example will guide the reader's thinking, for the sake of clarity.  While it is possible to continue explaining the steps using the example of the email application, the truth of the matter is that building an email application requires specific technical knowledge that will hinder more than help in the explanation of the problem solving process. Believe it or not, the problem of an email application can actually be a very vast one, so for the purposes of this course, and the remainder of this introduction, a simple problem will be sufficient to tackle.

The problem to tackle is that of deciding whether two numbers add up to a third number. This may sound like an astonishingly simple task, but that is a good thing, because it will allow the reader to concentrate solely on the problem-solving process. Now, recall that the goal of the engineer is to transform the problem into a series of inputs and outputs:

    INPUTS -> OUTPUTS

Thankfully, there are only a few clarifying questions that need answering. Firstly, can assume that numbers are real numbers. They can be positive or negative, or zero. We can assume the addition operator works as is normally expected of it. In short, there are reasonable assumptions to be made. Now, it is time to accomplish the task, and probably doing so would result in an understanding like this:

    Three numbers (a, b, c) -> True or False

This should make perfect sense. There are two numbers, and the desire is to know if they add up to the third number, and so the answer is either a “Yes” (True) or “No” (False). 

Now, to prove that we understand this, write some test cases that give correct sets inputs and outputs as is expected, for example this one:

    1,2,3 => True 

We know this is true because one plus two equals three. Here is another one:

    3,4,10 => False 

And a few more:

    -3, 0, 3 => False 
    -4, -4, -8 => True



Generating test cases in necessary and important. This is mainly because in real problems the engineer doesn't know how to transform the data from the inputs to the outputs. This being a simple problem, the reader can easilier see the answer, but that won't always be true. When this happens, the engineers needs to come up with more test cases, and often simpler ones. It may also be necessary to subdivide the problem. For the time being, we can be satisfied with the above test cases.

The next step is to brainstorm strategies. Maybe, in your mind, there is only one strategy, but to an engineer, there is always more than one way to do something. Here are a few ideas:

    1. Add the two numbers together, and compare the sum with the third number.

That is one way to do it, and here is another way.

    2. Subtract the second number from the third number, and compare it with the first number	

This solution is also valid. Some of you might think these two solutions are the same. Fundamentally, they accomplish the same thing, but they are not the same solution. This is because they are doing different mathematical operations, and this might be an important detail for an engineer. Once we get further down in the process, the basis for this claim will become clear. 

Lastly, it is important to note that while this problem had two very obvious solutions, there might certainly be more solutions. The end of this this course will cover strategies to come up with the solutions when no solutions come to mind. The technique for doing this is perhaps the most leastunderstoof of the engineer's skills, and it is still a field that the author personally feels is an area for significant academic research. 

In practice, coming up with solutions is hard because is requires the engineer to be aware of their down thoughts, and then be able to express, in words, how the inputs were transformed into the outputs. There are many strategies to help with this process, and they are outlined and the end of the chapter. This step is probably the most important. It is both a creative and disciplinary process - the former because insight is required, and the latter because attention to detail is required to put that insight into words. 

Having arrived at two solutions, the next step in the process is to pick one of them. To discern options is to weigh the trade offs. That is, when evaluating solutions, there will usually be pros and cons of each. Typically, there will be a trade off in terms of how quickly the solution runs. This is useful metric because users care about fast their computer programs run. Connecting this back to the two available solutions currently at the engineer's disposal, it is very possible that one of these solutions will run faster than the other because of computer's particular way of doing mathematical operations. That is, sometimes an addition operation will happen faster than a subtraction operation on a computer. This may be a trivial performance increase on a modern machine, but imagine a hypothetical scenario from a time in the past, when machines were very simple or rudimentary. In those situations, solutions could present very clear trade offs. In any case, it is simply enough to know that deciding on a strategy takes place in the problem solving process, and it’s important to know what the tradeoffs might be made when making that decision.

For our example, we will pick the first solution, and at this point, we come to the fourth step: 

    4. WRITE PSEUDO-CODE

Finally, a step involving the word “code” - but only pseudo-code. That is, code that is not really code, but more of an in-between of English and the high level programming languages known of today, such as Python, Javascript, Ruby, Java, etc. For our solution, we would probably describe it with the following:

    1. numbers a, b, c
    2. d = a + b 
    4. return d == c

Going line by line: in line one, we recognize that there are three numbers. In line two, we calculate the sum of the numbers, and in line three, we give the answer. What is above is pseudo-code because it looks like code, but is not formal syntax of any particular programming language. 

Now, moving forward, it is finally fair to say that the engineer needs be familiar with coding to write the above pseudo-code. They should have taken a codeAcademy course on a programming language of their choice. After taking that course, it won’t be hard to write pseudo-code. 

At the same time, writing peusdo can actually be one of the hardest things to do throughout this process. If it is hard, do more test cases until the process becomes so engrained in your mind that it flows out of you easily and quickly in words. 

There is also the problem of who exactly to write pseudo-code. My rule of thumb is to put every sentence into a line of code and subdivide the problem.

After having written pseudocode, implement the real code using the pseudo code as a guide. In order to do this, one needs to know how to code. That means: writing computer programs and running the program on a computer. For a student, they might write something like this:

    function TwoNumbersAddToThird(a, b, c) {
        return (a + b) === c;
    }   

This is an implementation in the programming language javascript. Even without any formal study in programming languages, the average reader can probably grasp how this function works, and how it relates to the peusdo-code above. If that is the case, then the read should be encouraged by his or her newly discovered abilities.  However, if the connection was not apparent, then it would be important for the reader to take a CodeAcademy intro. course on Python or Javascript. It will not be important for the student to be skilled at programming to appreciate this knowledge. In harder problems, the process of translating pseudo code into real code can be a truly arduous process, requiring hours of research into programming languages syntax, or deeply understanding the hardward that will ultimately run the code. 

Despite any challenges when going from pseudo-code to code, it is still the most colorful process of all the six, and this is because coding is a very messy process. ,Grit is not be undervalued here in this step. Perseverance is what empowers engineers to do what they call “DEBUGING” the code...that, being the process of writing code, running code, having the code churn out the wrong answer, then figuring out why it failed, and trying to fix it. 

Debugging takes takes an inquisitive mind, an inspector. In fact, amongst all the parts of building software, this particular process is the most stimulating for personally. There just something about the hunt for a bug. It is like that need to stractch an itch: the urge to scratch fills the body with energy and makes the body make the scratch, even if that person is a really tired and does not want to move at all.

Finally, if you test your code, and it works. Then congrats, you solved a problem! It is recommended to solve one hundred and fifty of these problems (Go onto either Codesignal.com or Leetcode.com). If you do that, and keep practicing until you can solve medium-level problems within forty-five minutes, then consider yourself a skilled coder, and apply for a job as a software engineer. Of course, that number is a rough estimate, casually recalled by the author as the number of LeetCode.com problems that the company Google thinks an aspiring engineer should solve before one is ready to interview. 

*An Exercise: (WANT TO KNOW)*

Think of a problem that you want to solve, and document your thoughts and conclusions as you go through problem solving process. It can be any problem; it doesn't have to be computer programming problem. That being said, it might hard to "implement" the solution to your problem, but you might come with something very implementable! 

Some questions to ask yourself are: Can I think of the problem in terms of inputs and outputs? Where do I get stuck in the process? What gets you unstuck?  

*Strategies: (LEARNED)*

Strategies that help along the various stages in the problem solving process:

1. Clarifying the problem and generating test cases, respectively: 
    - Ask clarifying questions and assume nothing.
    - Put yourself in a lot of situations where peers point out a test case that you hadn’t thought of yourself, and deal with the embarrassment that you didn’t think of it yourself. 
2. Coming up with strategies:
    If it is hard to come up with strategy, think first of more test cases and observe how they are similar to each other. Find the patterns. Write them down. If all of the test cases share something in common, then that information could be useful in how to get the inputs from the outputs.  Test out the observation by seeing if there is a way to explain how the output comes from the input, in terms of the observed similarity.  
    For example, lets say that I want to write some code that passes these three test cases, only these test cases, and no other test cases:
        
            [2, -1, 1] => [1, -1, 2]
            [3, -1, 2] => [2, -1, 3] 
            [3, -1, 0] => [0, -1, 3]

        You might start with some obvious things, such as the fact that every single array has three numbers, that the middle number is always -1, and that the inputs are unsorted, and the outputs are always sorted...that is, when we ignore the -1's. But this leads up to more intersting ideas. In fact,  just mentioning the -1 bears to light another striking pattern: that the -1's never move. At this point, some patterns are beginning to emerge in one's head, and so after having gone through this series of observations, it should now be clear that each test cases inputs simply have their first and last element swapped with eacher. As such, the logical step for this transformation is: 
    
            Swap the first element with the last element.
    
        This is a strategy, and arriving at this strategy is what is described above: it is way that a human being introspects their process of observation, makes note of key observations, and the combines them together to a series of instructions that turn the inputs into the outputs.

        How this is exactly accomplished by the mind is an academic interest for the author, but at this point, the only gauranteed way to do it is to subdivide the problem. This is the next technique to employ when having trouble coming up with strategies.

        Subdivision can be two things. Firstly, it can be used to explain how this partricular series of edge cases is really a subclass of a large series of test cases. 

            [2, -1, 1] => [1, -1, 2]
            [3, -1, 2] => [2, -1, 3] 
            [3, -1, 0] => [0, -1, 3]

            [-1, 4, 2] => [-1, 2, 4]
            [5, 0, -1] => [5, 0, -1]

        The first three tests are identical for the formers, and the next two are new cases of inputs and outputs. 
    
        Let us again make some observations. The new test cases are similar in structures (length, contain a -1, output is swapped, -1 does not move), but are also different in a single way: the placement of the -1. Pondering this fact, it should lead the problem solving to arrive at the observation that while the -1 might be placed elsewhere, the other two numbers to still simply swapped with one another. 
        
        But now, how to put all of this together into a pattern that accurately describes all of the test cases? How about:

            Swap the two numbers are not equal to -1.

        Which sounds easy enough, and viola, another strategy has bubbled to the surface. But remember, this conversation was about the idea of subdivison. Getting back to the concept, this brief digression showed how test cases could be subdivided and then built back to together to come up with more sophisticated strategies. How do we know that a strategie is sophisticated? We know when it can subdivided into multiple stpes. To understand, notice this strategy:

             Swap the two numbers not equal to -1.

        This strategy is actually two separate steps, written in one possily way as:

            First, find the location of -1. 
            Second, swap the other two numbers.

        Written another possible way as:

            First, find the two valid numbers
            Second, swap them.

        In either case, the reader should see how this problem subdivides. Unfortunately, it is insanely hard to see this connection, even for people learning to code. This is because the concept of moving things does not immediately appear to people as the two necessary processes of first finding the thing and then moving the thing. Yet, if people paid attention very closely, they would know that in their own life, whenever they want to move something, they must first locate it with their eyes, and then do the moving. Put another, it is possible to know that one must find something before moving something if evident in that fact that people fail to the find the things their looking for. 

        Consider, for instance, an hypothetical situation where you want to take out the milk from the fridge, but when you open the fridge to move it, you realize the fridge isn't there. If this happens, you will start wondering where the fridge is, but the only reason you care about it, at this point, at least, is because you want to move it. That is enough to convince the author that one must find before one moves, and this is very intimately tied together in the way the mind works, and programmer will study these structures and flows in the world of the mind and physical world when thinking of ways to subdivide problems. 

        Naturally, this kind of thinking occurs at larger and larger scales of complexity, at which case the computing machine itself becomes a source of intuition for how to subdivide problems, as well how to come up with test cases, and so getting back to the test cases under study, conclude this cases study by appreciating the two ways in which the concept of subdivision led to both the building up a more complex strategy, and to breaking down that same strategy, however deftly stated in words, into a pragmatic division of labor between separate processes. 
        
        Why such a subdivision of labor is necessary has not yet the subject of discussion, but now it will surface. In a nutshell, subdividing helps come up with more clear instructions when writing code. As it turns out, the subdivided steps are implementable while the single-sentence equivalent is not. The way that one knows that is by knowing what one's programming language of choice is capable of doing. This come from taking a quick course on a programming language, and then being capable of reading documentation about what programming software is available. 
        
        That is to say, if my manager asked me as to write software that did exactly as the aforemention strategy under analysis did, I would find someone who already wrote it online and just use that, because why would I need to reinvent the wheel? But, in the situation that I can only use a restricted resource, namely, only the programming language and no outside tools, I would have to write a program. As it turns out, I would have to subdivide my code into the chunks of code that the programming language is capable of doing.
    
        In other words, software engineers use subdivision to break a strategy down into logical steps they can code, and they use insights drawn from their observations of reality and the world to lend them insight into ways of subdividing the problem. Some of that may or may not have made sense, but hopefully it is clear that strategizing is very cognitive..

3. Pick a solution: Be evaluated on your judgement many times over and over again. Learn about Time and Space Complexity.
5. Implement and Test: Lots of coding and reading solutions.
    - First, take a Programming Langauge Course on Codecademy.com.
    - Second, if figuring out the code is a challenge, try letting an idea pop into your head. It will usually be just an inkling, so be sure to flesh it out as completely as possible.  The truth is that people have ideas before they understand them. Therefore, strive to implement ideas that come to mind, and seek to understand completely. For better or worse, this will probably involve debuging the code. 
    - When an ambiguity in syntax comes up, then use one's research skills to find the answer. This ususally involves reading stackoverflow.com or using the documentation for the programming language of ones choice.
    - Additionally, a technique for reading solutions is to do the code out on paper. Do not take shortcuts. "Doing the code" means stepping through the code, line by line, tracking all the variables. If you do this, you will understand the code, and you will gain insight. The truth is that we often cannot understand code by reading it. We must debug the code or do it out by hand. 
    - Study everything about the machine that will run the program. In todays era, that machine is the personal computer. Understanding the machine that run your program will make it easier for you to program them.
	
