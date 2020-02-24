# For the Lay Audience: How Computer Programmers Think 

by Adrian Jewell (www.adrianjewell.com)

(Thank you for reading!)

*Introduction (Know)*

This treatise contains everything the lay person needs to know about how to become a software engineer. There is no doubt that software engineers are in high demand. As of late, the website LinkedIn.com, posted 335,000 software engineer jobs last weekend in the United States. It is the author's position that while there are there are 10000 coding courses on Udemy, and 7,020,000,000 results on Google, the opinions contained therein are the gems of knowledge one needs to develop skills in computer programming.

Trust in the author's opinion. He is a software engineer with several years of experience, an alumni of the AmeriCorps, and a concert pianist turned composer. He taught himself to code as a teenager, and did a coding bootcamp later several years ago to help himself break into the field. He worked in the industry, and also worked full-time as a coding instructor. During this time, he learned a valuable lesson:

    Planning correctly will allow the problem solver to easily teach him/herself anything programming-related.

The truth is that while the majority of online coursework teaches very specific and some highly marketable skills, they don't teach how programmers think. Just do a search on Google, and see the plethora of courses with titles like: 
“Intro to Python”,
“Intro to Machine Learning”, 
“Working with Kubernetes”, 
“Build a Javascript Web Application in seven days”. 
While these courses are useful and necessary, they teach the how but not the why or what. Instead, study the information in container herein, and you will be able to master any of the skills mentioned above, and more, in a very short time, without any hand-holding that usually happens in courses, and that will make you very powerful. 

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

A computer programmer must also answer these questions before building the application. Why is that? Well, it’s because these questions have more than one answer. Thus, the engineer must decide the answer, and there may be more questions worth asking and answering. Given the fact of the matter, one might notice that these questions are slightly more specific than the first questions that were asked earlier. Therefore, they fall under the category of “TEST CASES” rather than “CLARIFYING THE QUESTION,” but as iterated before: both categories are very closely related to each other. Writing these tests cases is extremely important, perhaps the most important part of computer programming. 

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

Now, moving forward, it is finally fair to say that the engineer needs be familiar with coding to write the above pseudo-code. They should have taken a codeAcademy course on a programming language of their choice. 

At the same time, writing peusdo can actually be one of the hardest things to do throughout this process. If it is hard, do more test cases until the process becomes so engrained in your mind that it flows out of you easily and quickly in words. 

There is also the problem of who exactly to write pseudo-code. My rule of thumb is to put every sentence into a line of code and subdivide the problem.

After having written pseudocode, implement the real code using the pseudo code as a guide. In order to do this, one needs to know how to code. That means: writing computer programs and running the program on a computer. For a student, they might write something like this:

    function TwoNumbersAddToThird(a, b, c) {
        return (a + b) === c;
    }   

This is an implementation in the programming language javascript. Even without any formal study in programming languages, the average reader can probably grasp how this function works, and how it relates to the peusdo-code above. If that is the case, then the read should be encouraged by his or her newly discovered abilities.  However, if the connection was not apparent, then it would be important for the reader to take a CodeAcademy intro. course on Python or Javascript. It will not be important for the student to be skilled at programming to appreciate this knowledge. In harder problems, the process of translating pseudo code into real code can be a truly arduous process, requiring hours of research into programming languages syntax, or deeply understanding the hardward that will ultimately run the code. 

Despite any challenges when going from pseudo-code to code, it is still the most colorful process of all the six, and this is because coding is a very messy process.Grit is not be undervalued here in this step, because it is what empowers engineers to do what they call “DEBUGING” the code...that, being the process of writing code, running code, having the code churn out the wrong answer, then figuring out why it failed, and trying to fix it. 

Debugging takes takes an inquisitive mind, that of an inspector. In fact, amongst all the parts of building software, this particular process is the most stimulating for me, personally. There just something about the hunt for a bug. It is like that need to stractch an itch: the urge to scratch fills the body with energy and makes the body make the scratch, even if that person is really tired and does not want to move at all.

Finally, if you test your code and it works, then congrats, you solved a problem! It is recommended to solve one hundred and fifty of these problems (Go onto either Codesignal.com or Leetcode.com). If you do that, and keep practicing until you can solve medium-level problems within forty-five minutes, then consider yourself a skilled coder, and apply for a job as a software engineer. Of course, that number is a rough estimate, casually recalled by the author as the number of LeetCode.com problems that the company Google thinks an aspiring engineer should solve before one is ready to interview. 

*An Exercise: (WANT TO KNOW)*

Think of a problem that you want to solve, and document your thoughts and conclusions as you go through problem solving process. It can be any problem; it doesn't have to be computer programming problem. That being said, it might hard to "implement" the solution to your problem, but you might come with something very implementable! 

Some questions to ask yourself are: Can I think of the problem in terms of inputs and outputs? Where do I get stuck in the process? What gets you unstuck?  

*A Discussion on Strategizing: (LEARNED)*

Lets say that I want to write some code that converts the following inputs into the following outputs:

    [2, -1, 1] => [1, -1, 2]
    [3, -1, 2] => [2, -1, 3] 
    [3, -1, 0] => [0, -1, 3]

What engineer will do is start with some easy observations, such as the fact that every single array has three numbers, that the middle number is always -1, and that the inputs are unsorted, and the outputs are always sorted...that is, when we ignore the -1's. But this leads up to more intersting observations. For example, observing the sheer presence of the -1 illuminates a subtler pattern: that the -1's change their position when an input changes to an output. At this point, explanations for how inputs are turned in outputs are beginning to emerge in one's head, and perhaps, it will become clear that each test case's input simply has its first and last element swapped with each other. More formally stated, the logical step for this transformation is: 

    Swap the first element with the last element.

The above is what engineers call a strategy, discovered via the process just described. That is, the way that a human mind introspects their own process of observation, makes note of key patterns, and the combines them together to an instruction or, series of instructions, that successfuly convert all of the inputs into the given outputs.

How this is exactly accomplished is of academic interest for the author, for the sheer fact that all of the author's creative pursuits include moments of clarity. That is, several seconds of sudden realization that a pattern exists here or there, the details naturally depending on the medium of art being pursued at that moment. This moment of creative insight is so satisfying and seemingly illusive a feeling that the author feel warranted to request an in-depth study of the phenomenon. Specifically, scientists should study the causal events that lead up the moment of clarity.

In software engineering, that particular moment is the instant where all of the patterns that the engineer had derived from his or her observations suddenly congeal into the series of instructions that must be performed to transform the input into the output. That moment is a feeling engineers love to have, and even more, why people love to have this feeling is also an important question that merits scientific investigation.

Now, once the engineer has come up with the strategy for a given set of inputs nad outputs, it is then their job to understand how to get a computer to actually do the work required of the strategy. Now, the engineer turns his or her attention to figuring out how to understand their own thinking in terms that will make sense with the way the computer works. The fact is that computers don't work the way minds work, but until that time comes, engineers have to perform the work of transforming an idea that expresses itself so naturally in a spoken language, to a series of instructions that the computer will understand. 

The author's opinion is that the only gauranteed way to successfully do this is to subdivide the problem.  As a matter in fact, there are two different ways to do it.  First, subdivision can explain how the partricular series of edge cases described above is a subclass of a larger series of test cases (albeit, only two more). 

    [2, -1, 1] => [1, -1, 2]
    [3, -1, 2] => [2, -1, 3] 
    [3, -1, 0] => [0, -1, 3]
    +
    [-1, 4, 2] => [-1, 2, 4]
    [5, 0, -1] => [5, 0, -1]

The first three tests are of course identical for the formers, and the next two are new cases of inputs and outputs. 

Let the reader once again make some observations. The new test cases are similar in structure (length, containing  a -1, output is swapped, -1 does not move), but are also different, but only in one single way: the placement of the -1. Pondering this should lead the problem solver to arrive at the observation that while the -1 might be placed in a different position, the other two numbers still simply swapped get swapped with one another. 

Putting all of this together into a pattern that accurately describes all of the test cases would amount to:

    Swap the two numbers are not equal to -1.

 Lo and behold, a new strategy is born, and let us understand how subdivision applies here. Looking at this strategy reveals how the initial strategy is buried within this new strategy.  If we think about it, we will see that if the position of the -1 was in the middle of the three numbers, then the swapping that occurs would be identical to the kind of swapping done in the intitial proposed strategy (that of simply swapping the first and last element.) But of course, if the position of the -1 isn't the middle number, then certain other kinds of swapping need to happen, for instance, perhaps the first and second element, as opposed to the first and last. Thus, it becomes fair to say that not only does the new solution encapuslate the first solution, but it account for other transformations of the inputs too. In this way, appreciate how this creation of a hierarchy of logical operations amounts to a kind of subdivision, in the way that a tree's branches divide as the tree grows; parent branches include all the children of the branches are "subdivisions" of the parent branch.
 
 So, in this way, subdivision speaks to how strategies are comprised a smaller, individually describable strategies. Notice, as well, the way in which an example from nature serves as the analogy to explain the use of the word subdivision, Indeed, it is very interesting how the natural world inspires the creative mind.
 
 Getting back to the topic of subdivision, it should now be clear how subdivision in the context of a strategy. But, notice here how the trajectory of this particular discussion move from discussion a smaller set to a large set of inputs, and similarly, how the strategy of the smaller set of inputs is a buidling block of the solution described by the larger set of inputs and outputs. All of this implies a movement from the simple to the complex. Yet, there is also be many times when the opposite is required. The goal of subdivision, then is to break down a strategy into its component parts.
 
 To understand how this works, return once again to the strategy under analysis:

    Swap the two numbers not equal to -1.

It may be possible that somebody simply asked an engineer to write a program performed the above task, and the engineer didn't know how to code it. At this point, what the engineer will do is attempt to break the problem into smaller chunks that they do know how to code. Given the above the strategy, the solutions to such a division would probably look like this:

    First, find the location of -1. 
    Second, swap the other two numbers.

Written another possible way is:

    First, find the two valid numbers.
    Second, swap them.

In either case, the reader should see how this problem subdivide very nicely. Unfortunately, it can sometimes be insanely hard to see this subdivision. This is because the concept of finding things before moving them does not immediately appear to people as a subdivion. Yet, if people paid attention very closely to their mind, they would know that in their own life, whenever they want to move something, they must first locate it. The reason that this is true is because people get nervous when they realize they lost the thing they were trying to move. 

Consider, for instance, an hypothetical situation where you want to take your favorite shirt from the dresser, but when you open the dresser to take it out, you realize it's not there. If this happens, you will start wondering where it is, but the only reason you care about where it is is because you wanted to move it. Certainly there are other reasons to care about where something is, but for the sake of this exercise, simply understand insight that the intention to move something, followed by the fact that not knowing where it is creates anxiety is enough to establish the psychological construct of the need to find the thing as a precursor to moving the thing. This is all to say that the programmer studies the natural world, drawing inspiration from when thinking of ways to subdivide problems (once again a reference to the natural world).

Continuing forward, the coder then finds a way to explain these strategies in the most practical way possible, with the two sudivided options referenced in the gutter:

    If the -1 is in first position: \\ find the -1
        Swap the second and the third elements. \\ swap
    If the -1 is in second position:
        Swap the first and the last elements.
    If the -1 is in third position:
        Swap the first and the second elements.

Notice here how the new instructions a certain kind of subdivision, a subdivision that brings the instructions into a physical realm, as if the person reading the instructions was looking at the numbers on a chalkboard or as blocks on the ground. Regardless, the reference to the physical act of tracking things emphasizes that inputs and outputs are physical things being manipulated in the physical world. The engineer needs to be very in tune with this physical world in order to be able to derive instructions of this sort from the previous instructions. 

Then again, notice how this kind of thinking is innate to human beings use of language. Remember, just a moment ago, when in my description of how the simpler inputs' solutions was contained within the strategy to the larger set of inputs' solution. That is, it was not hard to make that analysis in the context of the parent, but in the situation where one is first given the parent strategy without the subdivisions are given, it is actually very difficult to make those subdivisions oneself, wherein lies the gift of the talented problem solver, and then necessity to refer to the nature or one's life experience in the physical world of life for explanations of how to subdivide a strategy.

As a side note, what the reader just learned regarding challenge of subdividing down exemplifies what mathematicians call NP problems. NP Problems can time a long time to solve, but it is a very quick process to know whether a given possible solution is in fact an actual solution to the problem. Subdividing is this kind of problem because making subdivisions can take a long tiem, but given a set of possible subdivisions to any given strategy, it is easy to tell which ones are in fact correctly contained in the parent strategy.

At the same time, for a very knowledgeable reader, it will occur to the them that the subdivisions being described could in fact be subdivided more, perhaps into physical movements of the body or eyes, ad infinitum. It is the engineers job to know that this particular series of instruction is best suited for trasnforming into code, and any software engineer is have this knowledge from simply learning to code. 

So there, subdivision highlights the ways in which the engineer reaches an understand of their mental processes as they transform inputs to outputs. It also brings the engineer closer to the 'code', so to speak, so that implementing the strategy becomes easier. Certainly, the journey doesn't stop here for the engineer. In fact, it  just began, for the task ahead is now to implement their strategy. But as wise people have said, "Where there is a will, there is a way," so the engineer is not worried about how he or she will realize the vision. The programmer trusts in their research skills and resourcefullness.

Still, there are certain strategies the engineers employ while learning to code that are worth mentioning briefly. The first is debugging. When debugging, the engineer look at code very closely while it is running. This is a supremely important skill to master. The second skill is doing code on paper. The profound truth about software engineering is the software often cannot be understood when it is read or conceived. Therefore, the engineer must actually run the code on a piece of paper, step by step, inorder to fully understand the code. Literature for how to accomplish these two technique abounds, so the author will simply highlight their common usage when an engineer writes code or is learning the workings of a computer program written by somebody else. The tips below will help an individual get started in coding.

Tips to Get Started:

1. Take a free online coding course (Codecademy.com is good, python or javascript are good to start). 
2. Ask an engineer to teach you how to debug, do code on paper, and "research documentation."
3. Do problems on leetcode.com and codesignal.com ( for codesignal: arcade or interview problems).
4. Apply this problem solving process to the problems.