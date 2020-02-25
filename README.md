# For the Lay Audience: How Computer Programmers Think 

by Adrian Jewell (www.adrianjewell.com)

(Thank you for reading! Please offer feedback and edit suggestions if so inclined)

*Introduction (Know)*

This treatise contains everything the lay person needs to know about how to become a software engineer. In fact, it might be good idea for more people to go into the field because software engineers are in high demand. This is known because the website Linkedin.com, recently posted 335,000 software engineer jobs in the United States. Now, it is the author's position that while there are there are 10000 coding courses on Udemy, and 7,020,000,000 results on Google, the opinions contained herein are the gems of knowledge one needs to develop professional-grade skills in computer programming.

Trust in the author's opinion. He is a software engineer with several years of experience, an alumni of the AmeriCorps, and a concert pianist and composer. He taught himself to code as a teenager, and later on, did a coding bootcamp to help himself break into the field. He worked in the industry, and also worked full-time as a coding instructor. During this time, he learned a valuable lesson:

    Planning correctly will allow the problem solver to easily teach him/herself anything programming-related.

Study this document, and you will be able to master any skill in coding, and more, in a very short time, without any hand-holding that usually happens in online courses, and that will make you very powerful. 

*The Process:*

The fundamental skill is software engineering is reasoning about problems in terms of inputs and outputs:

    INPUTS -> OUTPUTS

This may sound simplistic or contrived, but actually it is not. To exemplify, let’s say that you want to build an app for your phone that lets you read emails. If you want to build this application, you will probably be envisioning yourself using the app, in a scenario such as this:

    As a user, I want to go on the app and view my emails.  
    
The above epression is how the software engineer thinks about that particular idea in his or her mind.  In actuality, this particular sentence isn’t actually saying anything different that what we originally said in the previous paragraph, but it additionally implies a greater degree of specificity. Let’s think for a minute about why that is.

To start, there are probably some other requirements for this phone app, such as:

    As a user, I want to go on the app and see my emails, and NOT OTHER PEOPLE’S. 

That addendum may have suprised a few people, causing them to respond like this: "Duh!"...Do not be so quick to react in that way. If somebody asked me to build that app for them, and he/she told me the first requirement:

    As a user, I want to go on the app and view my emails.

...I’d certainly ask him/her if the users wants to only see their own emails, or whether user want to see their emails along with other peoples emails. In reality, this is a valid question because the original requirement doesn’t specify, while the addendum in capital letters makes this clarification. This may be a contrived example, but the only reason for thinking that is because when people talk about viewing email, they automatically assume the idea is to only see their own personal emails. This kind of thinking, however, is what engineers call jumping to conclusions, and that’s something to always avoid in software engineering. 

Now, another thing that is probably true about the email app is this:

    As a user, I DO NOT want other people to be able to view my emails.  

This requirement might also be implied by the original statement, but it is actually not implied at all. Once again, in today’s world, people generally assume that emails are private and confidential, but it is very possible that this particular app does not treat emails as confidential information.

Now at this point, it is possible to see that clarification of requirements could go on for much longer, perhaps like this:

    As a user, I want to view my emails…
            FROM ANYWHERE IN THE WORLD,
            AND THEY SHOULD LOAD QUICKLY,
            AND ANY EMAIL I RECEIVE SHOULD NOT BE MODIFIED AFTER I RECEIVE IT.

Most people would expect an email app to meet these requirements. In fact, all of these mentioned requirements are very interesting and challenging software problems that engineers have tackled for many years, but that is besides the point. For now, simply understand that clarifying requirements is a major part of a software engineer's initial reasoning about a problem. However, this process of clarification is not the key skill in software engineering, but rather a tool to help the engineer succeed at the original task: viewing a problem in terms of its inputs and outputs. In the case of our example, the answer is as follows:

    (Username and Password) -> (Emails associated with the Username)

The reader should see how the original line of inquiry led the software engineer to decide on these inputs and outputs. In case is not clear, a brief explanation follows. The engineer chose the username as an input because it is a "unique identifier" for the user. That is, the username can identify the user in such a way that every user is distinguishable from every other user. Armed with a username, the email app can filter for only the emails associated with the user while excluding the others. The password, similarly, is the way that the application verifies that users are in fact who they say they are. In this way, only the user itself can view the emails associated therewith. Perhaps this may be obvious, but it is worth repeat that the choice of a username and password is at least one possible way to fulfill the requirements settled upon earlier in the clarification:
    
    - As a user, I want to go on the app and see my emails, and NOT OTHER PEOPLE’S. [solved with a username]
    - As a user, I DO NOT want other people to be able to view my emails.   [solved with a password]

The example ultimately highlights several things. Firstly, the reader can see how even something as commonplace and deceptively simple as an email application can require planning. Login screens are not that interesting, but they are pieces of software about which engineers seriously thought over, and the above discussion is just the beginning.  

Now, the name for everything that just happened is called:

    1. CLARIFYING THE PROBLEM

Clarifying the problem is the first of six steps in a problem solving process that any programmer will execute when he/she writes a computer program.  The remaining steps are as follows:

    1. WRITE TEST CASES (examples)
    2. BRAINSTORM STRATEGIES
    3. PICK A STRATEGY
    4. WRITE PSEUDO-CODE
    5. WRITE CODE
    6. VERIFY/TEST (ACTUALLY IS DONE THROUGHOUT THE WHOLE PROCESS)

It will take some time to explain this process, but rest assured that mastering this process will enable the reader to do software engineering. Now, also notice that both “WRITE TEST CASES” and “CLARIFY THE PROBLEM” claim are part of the first step. That is intentional because these steps are one and same, but with slightly different names and looks. 

Continuing with the example of the email application will illustrate this point. Recall the decision for inputs and outputs:

    (Username and Password) -> (The Emails associated with the Username)
    
Does the programmer have enough information to begin building the app? The answer is no, because more questions must be answered before any programmer get started. Some of these are:

    What is a valid username?
    What is a valid password?

    What happens when invalid credentials are entered?
    What happens when empty credentials are entered?

    How many of the users emails do we want to return? 

A computer programmer must also answer these questions first because these questions have more than one answer. Thus, the engineer must answer them, and there may be even more questions worth asking and answering. Given the matter, one might notice that these questions are slightly more specific than the first questions that were asked earlier. Therefore, they fall under the category of “TEST CASES” rather than “CLARIFYING THE QUESTION.” Let's reiterate: both categories are very closely related to each other, and writing these tests cases is extremely important, perhaps the most important part of computer programming. 

At this point, it is the author's hope that reader is becomming interested in the process of software engineering. The reader also may also notice that not coding has been done yet. Isn't programming about writing code? Yes, but not yet. Remember, this article's goal is to explain the process of computer programming, and computer programming actually starts with this process of trying to understand the problem as clearly as possible. Once the programmer understands the problem, then he/she will move onto the steps more related to coding. The remaining portion of this introduction with walk through those remaining steps, but in order to do so will require a new example. 

For sake of clarity, a different example will illustrate the remaining five steps in the problem solving process.  While it is possible to continue explaining the steps using the example of the email application, the truth is that building an email application requires specific technical knowledge that will hinder, more than help, in the explanation of the problem solving process. Believe it or not, the problem of an email application can actually be a very difficult one. So, for the purposes of this course, and the remainder of this introduction, a simpler problem will suffice.

That problem will be the task of deciding whether two numbers add up to a third number. This may sound astonishingly simple, but that is a good thing because it will allow the reader to concentrate solely on the problem-solving process. Now, recall once again that the goal of the engineer is to transform the problem into a series of inputs and outputs:

    INPUTS -> OUTPUTS

Thankfully, there are only a few necessary clarifications. Firstly, can assume that numbers are real numbers. They can be positive or negative, or zero. We can also assume the addition operator works as is normally expected. In short, these are reasonable assumptions to be made. Now, it is time to accomplish the task, and doing so would probably result in an understanding such as this:

    Three numbers (a, b, c) -> True or False

This should make perfect sense. Start with two numbers, and output whether or not add up to the third number, and so the output is either a “Yes” (True) or “No” (False). To prove one's understanding, write some test cases that give correct sets inputs and outputs, for example:

    1,2 , 3 => True 

This is clearly true because one plus two equals three. Here is another one:

    3,4 , 10 => False 

And a few more:

    -3,0 , 3 => False 
    -4,-4 , -8 => True

Never forget that generating test cases is necessary and important and challenging. Notice that the test cases take 0 and negative numbers into account. These are what engineers call "edge cases", because they are often unlike the usual test cases. As a rule of thumb. Always be on the lookout for edge cases. Often, they are the most informative examples. 

Another reason that generating tests cases is important is because it will often be the case that the engineer doesn't know how to transform the inputs into the outputs. This being a simple problem, the reader can easily see the answer, but that won't always be the case. When the engineer gets stuck, he/she needs to come up with more test cases, and often simpler ones. It may also be necessary to subdivide the problem. As an aside, subdivision will be the topic of in-depth discussion later on in the paper, but for the time being, it is enough to be satisfied with the above test cases and the simplicity of the problem.

After coming up with test cases, the next step is to brainstorm strategies. Maybe in your mind, there is only one approach to this problem, but to an engineer, there is always more than one way to accomplish something (maybe even software engineering itself!). Here are a few of them:

    1. Add the two numbers together, and compare the sum with the third number.

Here is another way.

    2. Subtract the second number from the third number, and compare it with the first number.

The second solution is also valid. Perhaps, it is difficult to see how the two solutions are different at all. Although it is true that they fundamentally accomplish the same thing, they are not the same solution. This is because they perform different mathematical operations, and this might be an important detail for an engineer. Do not worry how this could be so, for the basis for this claim will become clear once get further along in the process. For now, appreciate the creativity that goes into finding multiple solutions, even for something as trivial as this problem.

It is important to note that while this problem had two very clear solutions, there might certainly be more solutions, and it often the case, that no solutions come to mind during a problem. How to come up with solutions will also be a topic of in-depth discussion later on in the paper. The technique for doing this is perhaps the least understood of the engineer's skills, and it is still a field that the author personally feels is an area for significant academic research. 

In practice, coming up with solutions is hard because is requires the engineer to be aware of his/her own thoughts, and then be able to express, in words, a series of steps that describe the inputs being transformed into the outputs. It is both a creative and disciplinary process. The former is required because pattern recognition requires insight, and the latter describing that insight requires attention to detail. There are strategies to help with this process, and they are outlined later on the discussion.

Now, having arrived at two solutions, the next step in the process is to pick one of them. What this mean is to weigh the trade offs of solution over another. That is, when evaluating solutions, there will usually be pros and cons of each, so the engineer must do the work evaluating those pros and cons. Typically, there will be a trade off in terms of how quickly one solution runs over another, and this is a useful metric because users care about fast their computer programs run. Connecting this back to the two available solutions currently at the engineer's disposal, it is very possible that one of these solutions will run faster than the other because of the computer's particular way of doing mathematical operations. That is, sometimes an addition operation will happen faster than a subtraction operation on a computer, or vice versa. This may be a trivial performance increase on a modern machine, but imagine a hypothetical scenario from a time in the past, when machines were rudimentary. In that era, solutions such as these could present very significant trade offs. In any case, know that deciding on a strategy takes place in the problem solving process, and it’s important to know what the tradeoffs might be made when making that decision.

For our example, the engineer will choose the first solution, bringing him or her to the fourth step: 

    4. WRITE PSEUDO-CODE

Finally, a step involving coding...sort of. That is, code that is not really code, but more of an in-between of English and the most common programming languages is called pseudo-code. In pseudo code, the chosen solution would probably be described with the following:

    1. numbers a, b, c
    2. d = a + b 
    4. return d == c

Try to understand this, line by line. In line one, recognize the three numbers (yes, that is a step for reasons described later). In line two, calculate the sum of the first two numbers. In line three, evalulate whether the sum equals the third number...it's pseudo code because it looks like code, but is not formal syntax of any particular programming language. 

At the same time, writing peusdo can actually be one of the hardest things to do throughout this process. If it is hard to come up with pseudo-code, the engineer probably didn't think clearly enough about strategies, and might need to subdivide the problem. In any case, do more test cases until the process becomes so engrained in the mind that it flows out easily and quickly in words. 

There is also the problem of how exactly to write pseudo-code. A rule of thumb is to put every sentence into a line of code and subdivide the problem. 

After having written pseudocode, implement the real code using the pseudo code as a guide. In order to do this, one needs to know how to code. That means: writing computer programs and running the program on a computer. For this problem, since the problem is trivial, the code will also be trivial:

    function TwoNumbersAddToThird(a, b, c) {
        return (a + b) === c;
    }   

This is an implementation of the solution in a programming language called javascript. Even without any formal study in programming languages, the average reader can probably grasp how this function works, and how it relates to the peusdo-code also written above. If the read grasped the connect, then he/she should be encouraged by his or her newly discovered sense.  However, if the connection was not apparent, then it would be important for the reader to take a CodeAcademy.com introductory course on Python or Javascript and then revisit this example. That being said, it is not necessary for the student to be skilled at programming to appreciate this knowledge, but know that in harder problems, the process of translating pseudo code into real code can be a truly arduous process, requiring hours of research into programming languages syntax, or deeply understanding the hardward that will ultimately run the code. 

Despite any challenges when going from pseudo-code to code, it is still the most colorful process of all the six, and this is because coding is very messy. Grit is not be undervalued here, because grit enables engineers to do what it called “DEBUGGING”  code...that, the the process of writing code, running code, having the code output the wrong answer, then figure out why it failed, and try to fix it. 

Debugging takes takes an inquisitive mind, that of an inspector. In fact, amongst all the parts of building software, debugging is most fun for the author personally. There just something about the inspection of broken software that energizes the body. It is like the urge to stractch an itch: the urge to scratch fills the body with energy and makes the body perform the scratch, even if that person is really tired and does not want to move at all. With code as well, if the engineer wants to find out why something broke, he/she will often not stop until he/shes figures it out.

After all that debuggin, if the engineer tests his/her code and it works, then congrats, the problem is solved! For the aspiring engineer, solve a minimum of one hundred and fifty of these kinds of (log onto either Codesignal.com or Leetcode.com to find problems). After that, keep practicing until solving medium-level problems within forty-five minutes is easy, then apply for a job as a software engineer. Of course, that number is a rough estimate, casually recalled by the author as the number of LeetCode.com problems that Google thinks an aspiring engineer should solve before one is ready to interview. 

*An Exercise: (WANT TO KNOW)*

Think of a problem that you want to solve, and document your thoughts and conclusions as you go through problem solving process. It can be any problem; it doesn't have to be computer programming problem. That being said, it might hard to "implement" the solution to your problem, but you might come with something very implementable! 

Some questions to ask yourself are: Can I think of the problem in terms of inputs and outputs? Where do I get stuck in the process? What gets you unstuck?  

*How To Brainstorming Strategies: (LEARNED)*

Lets say that I want to figure out how the following inputs convert to the following outputs:

    [2, -1, 1] => [1, -1, 2]
    [3, -1, 2] => [2, -1, 3] 
    [3, -1, 0] => [0, -1, 3]

If the engineer doesn't know the answer, he/she will start with some easy observations, such as that every single array has three numbers, and that the middle number is always -1. This will naturally lead to the observation that those two nonnegative inputs become sorted in the process of an input changing into an output. These observations lead to even more intersting observations. For example, presence of the -1 illuminates a subtle pattern: that the position of the -1 changes when an input changes to an output. From these collective observations, the explanation for how inputs turn into outputs will begin to crystallize in the mind. Perhaps, it is not clear that each test case's input simply has its first and last element swapped with the other. More formally stated:

    Swap the first element with the last element.

The above statement is an example of what engineers call a strategy, discovered via the process of making more and more sophisticated observations, ending in the discovery of how the input becomes the output. Regarding the actual strategy, it should be a relatively quick procedure to verify that it actually does describe all the test cases, so see that it does. Regarding the process of arriving at the strategy, the author has no clue what happens in the brain when an engineer arrives at a strategy. The author did attempt to eloquently describe a theory of the mental mechanism involved in such a task, and what he came up with reminded him of the ideas he and his friend thought up when they took LSD together. In short, the mind works in a recursive way, described best with geometic designs. In truth, I have no idea what happens but I am dying to know, for I cannot see what happens in the brain. 

Therefore, how this is exactly accomplished is of great academic importance, for the sheer fact that all artistic pursuits include these moments of clarity: several seconds of sudden realization that a pattern exists, the details of which are, of course, naturally dependent on the medium of art being pursued. This moment of clarity is so satisfying, yet so illusive a feeling that the author feel warranted to request an in-depth study, should one not exist. 

In case it wasn't clear, that particular moment in software engineering is the instant where all of the patterns that the engineer had observed from his or her observations suddenly congeal into the series of instructions that must be performed in order to transform the input into the output. In fact, the beautiful and desirability of this feeling is such that author also requests a thorough study of why people seek to have this feeling.

Now, once the engineer has come up with a strategy for transforming a given set of inputs into outputs, the job is now to write out the strategy in a way that a computer can understand the instructions, thereby performing the work contained therein. To do this, the engineer turns his or her attention to to understanding his/her own thinking in a new way. Once again, the author has no clue how the brain does this, so here again is an opportunity for to provide some additional thoughts on what it takes to do such a thing. Yet again, the words bore a striking resemblance to the intellectual musings that arise when immersed in the psychedelic experience of reality bending in strange loops. That is to say, it's pretty trippy to think about this kind of stuff. And the truth is that this work, this carefully rethinking of one's own thoughts, is a laborious process.  Until that time comes when it is not, the engineer has to just do it. While there will hopefully come a time when coding is an effortless process, the mental labor of translating language into code is quite mysterious, in and of itself; despite the strong desire to alleviate it as much as possible, the miracle of the mind being able to it in the first place, yet be avoidant to it, and also be able perform amazing feats of resourcefullness through it, all at the same time, merits an academic investigation of large scale. At least, please stop fighting wars and put resources into answering questions like these.

The author's opinion is that the only guaranteed way to successfully make this translation is to subdivide the problem. Getting there, however, will require some preliminary thoughts. Let us first see how subdivision will help explain how the partricular series of edge cases described above is a subset of a larger group of test cases (albeit, only two more). 

    [2, -1, 1] => [1, -1, 2]
    [3, -1, 2] => [2, -1, 3] 
    [3, -1, 0] => [0, -1, 3]
    +
    [-1, 4, 2] => [-1, 2, 4]
    [5, 0, -1] => [5, 0, -1]

The first three tests are of course identical for the former, and the next two are new cases of inputs and outputs. 

Let the reader once again make some observations. The new test cases are similar in structure (length, containing  a -1, output is swapped, -1 does not move), but are also different in one single way: the placement of the -1. Pondering this should lead the problem solver to arrive at the observation that while the -1 might be placed in a different position, the other two numbers still simply swapped get swapped with one another. 

Putting all of this together into a pattern that accurately describes all of the test cases would be:

    Swap the two numbers are not equal to -1.

 Lo and behold, a new strategy is born, and let the reader understand how subdivision applies here. Looking at this strategy reveals how the initial strategy is buried within this new strategy.  Thinking will show that if the position of the -1 was in the middle of the three numbers, then the swapping that occurs would be identical to the kind of swapping done in the intitially proposed strategy (that of simply swapping the first and last element.) Of course, if the position of the -1 isn't the middle number, then certain other kinds of ways swapping would need to happen...for instance, perhaps the first and second element would be swapped instead. Thus, it is fair to say that not only does the new solution encapuslate the original solution, but it accounts for other transformations too. In this way, appreciate how this creation of a hierarchy of logical operations amounts to subdivision much in the way that a tree trunk branches off into many more than were started with.
 
 In this way, subdivision speaks to how a strategy is smaller, individually describable strategy of a more complex strategy. Also notice that an example from nature serves as the analogy to explain the use of a technical concept. So, it should be generally clear how subdivision works, but before saying anything else, notice the trajectory of this particular flow in the discussion. Notice how the discussion led the reader from a discussion of a small set of input and outputs to a larger set, and similarly, how the strategy of the smaller set of inputs is a portion of the solution described by the larger set of inputs and outputs. In short, it is a movement towards the complex. Yet, there are times when the opposite is required. In these cases, the goal of subdivision is to break down a strategy into its parts.
 
 To understand, return once again to the strategy under analysis:

    Swap the two numbers not equal to -1.

It may be possible that somebody simply asks an engineer today to write a program to perform the above task, and the engineer doesn't know how to code it. At this point, the engineer will attempt to break the problem into smaller chunks that he/she does know how to code. How this is done will now receive a demonstration. 

Given the above the strategy, the solutions to such a division would probably look like this:

    First, find the location of -1. 
    Second, swap the other two numbers.

Written another possible way is:

    First, find the two valid numbers.
    Second, swap them.

In either case, the reader should see how this problem subdivided very nicely. Unfortunately, it can sometimes be insanely hard to see this subdivision. This is because the concept of finding things before moving things is not apparent as step in people's minds. Yet, if people paid attention very closely to their minds, they would know that in their own lives, whenever they want to move somethings, they must first locate them. The reason that this is true is because people get nervous when they realize they lost the things they were trying to move. 

Consider, for instance, a hypothetical situation where you want to take out your favorite shirt from the dresser, but when you open the dresser to take it out, you realize it's not there. If this happens, you will start wondering where it is, but the only reason you care about where its whereabouts is because you want to move it. Certainly there are other reasons to care about where is located, but for the sake of this exercise, simply understand that the anxiety of not knowing the whereabouts of an object one wants to move establishes the psychological construct of the need to find the thing as a precursor to moving the thing. This is all to say that the programmer studies the physical nature of things, drawing inspiration from it when thinking of ways to subdivide problems. In fact, the author is very interested in exploring the connection between this physical world in the mental world and the actually physical world, on the basis of the above claims.

But continuing forward, the coder will a find ultimately find a way to explain the strategy in a practical way such as this (with the two sudivided options referenced in brackets:)

    If the -1 is in first position: [find the -1]
        Swap the second and the third elements. [swap]
    If the -1 is in second position:
        Swap the first and the last elements.
    If the -1 is in third position:
        Swap the first and the second elements.

Notice here how the new instructions demonstrate certain other kind of subdivision, a subdivision that brings the instructions into a physical realm, as if the person reading the instructions was looking at the numbers on a chalkboard or as blocks on the ground. Regardless, the reference to the physical act of tracking things emphasizes that inputs and outputs are actual things being manipulated as they existed in a physical world. 

Then again, notice how the discussion already spent some time in referral to a process such as the one described above. Remember just a moment ago, the description of how the simpler inputs' solutions was contained within the strategy to the larger set of inputs' solution. It was not hard to make that analysis in the context of considering a child's relationships to the parent, but in the situation where one is first given the parent without the subdivisions, it is very difficult to make those subdivisions oneself. To aid along the process, refer to nature or one's life experience in the physical world of life for examples of how to subdivide a strategy.

As a side note, what the reader just learned regarding the challenge of subdividing down exemplifies what mathematicians call NP problems. NP Problems can time a long time to solve, but it is a very quick process to verify a possible solution. Subdividing is a kind of this problem because making subdivisions can take a long tiem, but given a set of possible subdivisions to any given strategy, it is easy to tell which ones are correctly contained in the parent strategy.

At the same time, it will occur to the very knowledgeable reader that the subdivisions being described could in fact be subdivided more, perhaps into physical movements of the body or eyes and more detailed biological processes in the human body, etc. It is the engineer's job to know that which 'level' best suited for trasnforming into code, and any software engineer will gain this knowledge by simply learning to code. 

So there, subdivision highlights the ways in which the engineer reaches an understanding of his/her mental processes as he/she transform inputs into outputs, and brings the engineer 'closer to the code' so that implementing the strategy becomes easier. Certainly, the journey doesn't stop here. In fact, it just began, for the task ahead is now to implement the strategy. But that will not be part of this discussion, for it is enough to say as people have said, "Where there is a will, there is a way." In this way, the engineer is not worried about how he/she will 'realize the vision.' The programmer trusts in his/her research skills and resourcefullness.

Still, it is worth mentioning certain strategies that the engineers employ while learning to code. The first is debugging. When debugging, the engineer look at code very closely, while it is running. It is supremely important to master this skill, but also an important to master doing code on paper. The profound truth about software engineering is that software often cannot be understood when it is read or written. Therefore, the engineer must actually run the code in his/her mind, step by step, in order to fully understand the code. Literature for how to perform these two technique is abundant, so the author will simply highlight their common usage. With that, this concludes the discussion on how programmers think. Thank you again reading, and please leave feedback!

The tips below will help an individual get started in coding.

Tips to Get Started:

1. Take a free online coding course (Codecademy.com is good, python or javascript are good to start). 
2. Ask an engineer to teach you how to debug, do code on paper, and "research documentation."
3. Do problems on leetcode.com and codesignal.com ( for codesignal: arcade or interview problems).
4. Apply the ideas in this paper to the problems.