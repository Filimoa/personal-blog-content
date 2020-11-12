I've come to learn the best way I pick up new skills is by diving into projects I'm passionate about and fill in the theory later. For me, this goes for everything from fitness to software frameworks. [transition]I'm not sure why but I've always had a fascination with weather. As a kid there's a sense of wonder that I got watching storms pass over or trying to predict snow days. When I got to college I started learning about complex systems - one of which is weather. To put it simply, these are systems that have deeply interwoven inputs that make them impossible to predict. As a result, believe it or not, a butterfly flapping it's wings in India has a non zero chance of causing a tornado in Kansas.

Even with the fastest supercomputers on earth, we still can't predict the weather more than a few days out . This became a real problem for me when I tried to plan snowboarding trips. The goal of which was to always being to catch a big storm and ride fresh 'powder'. Until you've done it yourself, it's hard to describe the sensation that comes with getting 'first tracks' across last nights storm.
With the closest mountain being located hours away, living in Ohio means that kind of trip takes some planning. To make matters worse the forecast for each resort, and there's lots of them, is on it's own website. This means hours of navigating webpages with the chance you'll have to redo everything tomorrow when the forecast inevitably changes.

To me, a solution here seemed obvious - an interactive map that displays the forecast overlaid with the nation's ski resorts. Too bad this didn't exist. Maybe I could make it? Probably not, I was just starting to get a handle on Python - front end web development was not a bridge I was ready to cross. But when you have a hammer, everything looks like a nail so I set out to make it in Python. Weeks go by. If you know anything about coding this was a terrible idea so as you might expect I didn't get very far - you can see the earliest version below.

[PYTHON V1 PIC]

But this left me hopeful. I didn't touch the project for over a year and I eventually graduated from college [started work at Honda]. Now I'd have the disposable income to go on more snowboarding trips. Too bad every single time I have to plan one I'm left frustrated with the amount of time I spend on Google. [Feeling of wanting something and knowing you can build it -> better transition] Around August I decide I'm going to take the plunge and like any good student developer, use this an 'opportunity' to learn a front end framework.

After a few weeks of harassing every tech person I know about building websites I settle on learning React. Initially afraid of the commitment, I send out a couple hundred surveys in Facebook snowboarding groups hoping I'm not the only one with the problem. In addition to learning some people snowboard over a 100 days a year - slightly jealous - I find out others are in fact deeply dissatisfied. Seems great, now I'd just need to figure out how to make it. I come up with a plan where I'd code three versions of the site, starting from what was basically a list with pictures and working my way up to the actual interactive map to be launched into the world. Learning from my past failures, breaking down the problem into smaller chunks goes a long way in helping me avoid burnout.

[EARLY WEBSITE]

React ended up being an absolute pleasure to learn with some of the best documentation I'd ever come across. Coming from a background of physics, it scratched a deep itch of creating something that's elegant. Better yet [need to add repetition and something about taste]
At some point I was going to have to figure out how to display the forecast. At first I subdivided Colorado into small squares which was tedious to code and doesn't come out looking right. After some searching I came across a library that's based on hexagons - which look nice and simplify the code. So I took the outline of Colorado and split it into 7000 hexagons. Then I wrote a script that could call the forecast for each hexagon and bin hexagons with similar amounts of snow into one shape.
See the difference below, this reduced the memory footprint by 90%. It could also take the historic data that I was saving and create forecast for past accumulation. That way if you're coming into a resort you could get an idea of how much snow had recently fallen.

[PICS OF HEXAGONS]

Once I launched I started getting some interesting feedback. I found this to be one of the most rewarding parts of this project - seeing people actually using it. It was clear some parts of the website would need to be clearer. For example it used to be that searching a resort doesn't trigger an update until you clicked out of the search bar causing users to think it was broken. Small details like this can have massive impacts on accessibility.

![User Testing](https://github.com/Filimoa/personal-blog-content/blob/main/blog/powdamap/user-testing.jpg?raw=true)

As I wrap up the project I can comfortably say I have handle on react and have learned magnitudes about the software development lifecycle. I'm going to try to clean up the code in the next few months and open source it on GitHub. In the meantime please feel free to reach out if you have questions on it.

[FINAL SCREENSHOT]
