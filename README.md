# ScheduledHarmony #
This is an algorithm for scheduling classes at my former high school that I worked on for over a year and a half. It takes information about student forecasting requests and the classes each teacher is anticipated to teach. Using this data, the algorithm attempts to place students into groups with a given size and assign a teacher to each group. This program is expected to save hundreds of hours spent by staff placing students into classes, as well as increase the percentage of forecasting requests that are granted.

## Documentation ##
In this GitHub repo, you can find a comprehensive instruction manual on how to use the program. This manual is intended to be used by someone with basic knowledge of scheduling high school classes, but not necessarily any computer science experience (eg. a high school counselor). Unfortunately, no further documents or code are available for public viewing at this time.

## What I Learned ##
Working on this project for a year and a half makes this by far the largest project I've completed. Over those two years, I had to constantly re-factor my code to align with new things I was learning about proper C++ programming style. With little formal instruction, most of the knowledge needed for this project was self-taught.

Given these defining characteristics of this experience, I learned:
- How to develop a complex algorithm given unique constraints.
- How to select an algorithmic technique for a specific task.
- How to manage and remain accountable for a large project.
- How to properly employ object-oriented programming to organize a large project.
- How to work with a client's constraints and data formats to provide a user-friendly interface.
- How to parse and process large quantities of data.
- How to document use of a product.
- How to code proficiently in C++.
- How to compile code with CMake.

## The Design Process ##
### Inspiration ###
For my high school of around 1600 students and 90 teachers, scheduling each year's classes was an incredibly lengthy project. The counselors would spend hundreds of hours anually at whiteboards and computers arranging classes into a schoolwide schedule based on student forecasting requests. Further, several counselors cited this as one of the least desirable duties associated with the job. And considering the scope of the problem, it was difficult for the counselors to consider enough unique schedules to find a close-to-optimal solution. I was intruiged by the complex nature of the problem and excited by the prospect of creating such a useful program. So when the counselors approached my CS teacher with the idea of an algorithm for scheduling classes, I asked to be a part of it.

### Planning ###
Myself and one other student were the ones to step up to the challenge. So we spent the next several weeks researching possible algorithms, discussing their limitations, and debating their effectiveness. In retrospect, I think we could have benefited from even more time spend theorizing and planning. But at the end of this extended brainstorming, I had a fairly detailed idea for how to structure the algorithm. This idea ended up being almost exactly how the final implementation works. The general concept is to assign a quantitative value to how good a certain schedule is, then try to optimize that value.

### Creation ###
I started working on the project alone. Myself and the other student decided to attempt different methods of solving the problem. They would graduate at the end of that year, leaving only me working on the project. I decided to use C++ because of its efficiency, so I had to familiarize myself with the language. This process ended up going on alongside writing the code, with the codebase going through multiple revisions based on newly learned information about best C++ practices. I also had to select a specific linear programming algorithm to implement, which took even more research. Then began the actual coding of the project, a year and a half process full of logic problems and data parsing.

### Obstacles ###
One of the most initially obvious obstacles would be maintaining motivation throughout the project. However, this wasn't too much of an issue for me. The problem was quite interesting and the occasional breaks for other coding assignments provided a bit of variety. I would often work on it outside of my computer science class, which proved to be essential to completing it by graduation. The other obstacles were somewhat more technical in nature. I had to find a way to optimize for both student requests and teachers' classes, accomodate both year-long and semester courses, parse and deduce poorly structured data, and just keep track of the substantial codebase.

### The Result ###
I finished the project just after my graduation, before the end of the school year. Based on my initial testing on data from a previou year, the algorithm was quite successful. While the councilors' previous class placement was below 7 in 8, the algorithm gave students an average of 7.1 in 8. While I don't have the exact statistics yet due to lack of data, these results seem to indicate at least 1 additional class request granted per 5 students. And while the final schedule produced by the algorithm will still needed to be adjusted manually to account for specific niche cases, it should save many of the hundreds of hours previously spent on scheduling. My high school councilors are very excited to put the program into use this year, and I'm eagerly awaiting news about the results of my work.
