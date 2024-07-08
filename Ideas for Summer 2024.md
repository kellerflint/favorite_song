
Recording thoughts:
[If You Want A Better Sounding Voice, Do THIS Instead. (youtube.com)](https://www.youtube.com/watch?v=ghig3bqAwqM)
[Public Speaking: How To Make An Audience Love You In 90 Seconds - YouTube](https://www.youtube.com/watch?v=k8GvTgWtR7o)

>When you first start to study a field, it seems like you have to memorize a zillion things. You don’t. What you need is to identify the core principles – generally three to twelve of them – that govern the field. The million things you thought you had to memorize are simply various combinations of the core principles.
>- John Reed


Maybe the way to approach the peer reviews is to make these assignments fairly short and scenario based. Given this problem, solve it. That way no one is having to grade a ton and it makes sense to mostly base them on completion. It would also be easy for you to skim them if there fairly short.

- [Learn Database Normalization - 1NF, 2NF, 3NF, 4NF, 5NF - YouTube](https://www.youtube.com/watch?v=GFQaEYEc8_8)

[ARCS Model of Motivational Design Theories (Keller) - Learning Theories (learning-theories.com)](https://learning-theories.com/kellers-arcs-model-of-motivational-design.html)

Maybe we can have them just have 1-2 databases that we work with in class in PHPMyAdmin. That way they can just create databases for those and keep them rather than constantly adding and re-dropping. And then one workspace database that they can use to create their own stuff.

Probably Northwind and one other. Maybe not Magic Store, I should make a new / fun / different one I think.

There are two broad categories of change I'd like to make to the class: Lessons and Assignments.

Actually the biggest thing I need to do with lessons is just plan them out a lot more cohesively. At this point they're a bit of a mix of different quarters I've run things. I've also never had a whole plan from beginning to end. I think this creates confusion and weirdness.
- What we need
	- Each week should flow easily into the next week. They should build very clearly and deliberately. Right now it's a bit like I introduce a bunch of concepts in a week and then more in another week, but the clear line through them isn't necessarily there, I think to a struggling student the progression of their understanding is not good, it's a little haphazard. I need to come up with an actual concept map so I know exactly what I'm developing in what weeks and how deep their understanding should be at any given point.
- (I made a video to explain the problem to you. It's called 2024-04-29_11-12-51 in OBS OUT right now)

- ALSO I should do the learning objectives KT thing for SQL too, that's a good idea. If we go in person I'll probably make them do entry or exist tickets too just like this one.

First, I'd like to make the lessons deeper and give more visual examples. I'd also like to include additional optional videos / resources for students who are struggling or confused. I think you need a few practice questions WITH answers that they can see on their own. I also should have videos where I show in a very clear and methodical way how to do things like submit assignments and do an actual like split screen example.

Second, I'd like to make the practice assignments more helpful. They should all have images of the expected results so it's clear to students what they should be getting. It'd be great if I could then implement an AI feedback mechanism so I can quickly grade them and give comments. 

I also think I should make the databases for both practices and assignments more interesting. We should see if we can find platforms (like the google query one) where they can write SQL and explore real data. We should have an assignment somewhere in here in which they also get to choose more of their own data sets.

Fully automated or AI grading for all of the practices and AI assistance for the assignments would be super helpful as well and would probably not be wasted time since. I'm hoping that I can hold on to 201 in the very long term and the good news is SQL doesn't change much. So as long as we're still doing it most of my content should start staying 100% the same.

I don't feel like I need a ton of interactivity personally (it's on online async class, it's just not the best environment for it imo. We'll bring it in-person or hybrid if this is necessary). But one thing I could do is write a custom message for each of the weekly updates / check-ins. Actually introduce the topic in a few sentences and have these locked and loaded so I just need to update dates before sending them out.




How to do grading for 201.

Here's what you do. Write a script that initializes the DB.
Then it runs the example query against their query. If the results are the same it outputs that it passed. If they're different or missing, it outputs a fail.
- Do a little pre-processing, have it remove any line that starts with a --.

If it fails on anything, have the AI take a pass at it, see if it can determine feedback on the ones that failed. Or if no feedback is needed and the query looks correct even though it failed, just mark it as fine.
- Give the AI the answer key and the results that their query returned (or none if none). The tool won't know why something failed but the AI will. So if it's weird and they only submitted like 3-8, the AI should be able to pick that up and comment it.

Also have the AI highlight any student questions from the text. Have it answer them and let me know at the end.

Then output a report with each student first_last name, the status of each question of if it ran successfully or not, and the AI's feedback. You could literally copy paste this into Canvas. I bet it could literally take maybe 15 minutes to grade 24 students.


Another good auto grading idea - have them submit video things. Then have AI transcribe them, summarize it, and compare it to a rubric. That would also be pretty effective. And just review any weird cases.


Oh and for mastery based learning, AI can literally supply infinite variants of the same questions. Easy lol.


I want to think through, maybe with Ken, how mastery based class could be done at a college.






Reframing the content. Build from the ground up. Assume we intro level things they way you used to do in your old HTML / CSS / JS tutorials.

What even is data? What even is excel? What does it mean to organize data into columns? What is data analytics? Why do we care at all? Stuff like that
- Visuals for all of this

New lessons sequence
- How the course is structured. Do multiple videos on this. Start with how to use canvas. How to submit things. Where to find your lessons and how they work. Clear idea of the grading scheme, approach and policies. Where can you get support and resources? Go through all of this.
- Then what is in our course? Do a better overview. Instead of just listing topics, give them a super high level understanding of what each week actually is. Like I can show them the kind of things they'll be able to do by the end of each week and give broad definitions of everything so they sort of have the mental framework already there.
- What is data? Tabular data definition. Reading a spreadsheet in something like excel
	- This may be an extremely basic overview. But remember, the best learning happens when you're seeing content for the 2nd, 3rd or 4th time. When you have some ideas already of where it sits. It's a good chance to make sure you are up to speed and check that you do actually understand the basics. Often you will be missing some small thing or have some realization about how data is structured that you didn't have the first time. So try and stay engaged even with simple things.
- What is a database? Why do we need databases vs excel? What is a relational database? What is SQL? What does some of the syntax look like? Where does it sit in the web stack? How does it interact with other things they may already be familiar with? Like websites sending data back or an IoT device or whatever.
- Only now do we move on and not to actual relational concepts, but to basic selects and filtering. Incorporate the concept of EDA as well in these first weeks. Cover all the basic commands, so `SELECT` `WHERE` `ORDER BY` `DISTINCT` the operators, all these basics. Show very clear examples. Also, talk about what the data means. Ask them to explain what the data means. See if we can get GPT hooked up to quizzes in Canvas for auto grading of actual text to make sure they're getting the gist.
- Then next we should do aggregation and column aliasing. On systems with multiple tables but never JOINing, just one at a time.
- Then we do group by and having, again on single tables
- Then we do our first project, because now they can do analytics.
- Then basics of architecture. What it means for tables to be related to each other. Clear videos on PKs and FKs. Clear videos on one to many. This needs to be made clear through MANY examples. What it means for something to be one to many. Lots of practice reading a thing and deciding what the one side and many side is. Lots of examples showing how this is the case in the data, why it is one to many, the direction the relationship goes in because of how the table / columns are set up. And how you can understand the direction just from the table itself without a diagram.
- Then basics of ERDs. Show how we can represent these one to manys. Get into data types and diagraming tables to solve simple problems
- CREATE and INSERT
- Then many to many relationships. How these are represented. How they are different. Lots of practice understanding these 
- Then advanced querying topics. Start with JOINs. Show clearly what's happening in ERD from, from the data, show the query being built up step by step. Cover table aliasing
- Then sub querying (which I think is optional, can see how long it takes to get through the rest of it) and the final project / weeks on putting it all together. Have some kind of project / open assignment even if it isn't the final exam and just a final project.
- A cool alternative final exam format might be to give them a dataset and have them do EDA. Ask some high level questions and have them come back to you with answers. Open note of course, though not open GPT.

Notes
- Where we can provide additional resources or someone who does a good visual or explanation we should. You can make them required if you feel it's good enough, that's totally fine you don't have to reinvent the wheel on everything if someone else has done a good job visualizing or explaining a topic. I think providing additional deep dive material each week would also be good.
- Where we can we want to provide automated and early feedback. Maybe through your query checker site idea or even through showing the expected results. I think both approaches are fine, though the query checker is cooler and could maybe integrate a touch of AI. But you shouldn't do this unless it's pretty easy for you. It could even be a "does my script run successfully" checker. You could tell them it's doing a basic validation pass, checking that it ran and the expected count of rows were returned but remind them that it is not the same thing as being right, its just an approximation. This is why we probably need to include expected results too. You know if you wanted these could all be in one place, this site could check and tell them what it was supposed to return by actually running your answer key queries and showing them. It would make it super easy for you to update / mod in the future too.