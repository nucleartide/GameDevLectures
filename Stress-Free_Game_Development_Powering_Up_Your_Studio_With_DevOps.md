> https://www.youtube.com/watch?v=t9HRzE7_2Xc 

* Three ways of devops
* Solo operation
* Crashlands
*  Art asset pipeline
    * Artist: create asset, export asset
    * programmer: import asset, review asset, report errors
    * artist: fix errors
    * programmer: implement asset
    * The inkbot
* Development continues like before
    * You can get away with bad process on a small team
    * What is launch going to be like?
* Life after devops
    * Levelhead 97% positive
    * 2-3 content patches a month
    * Up to 4 patches deployed to internal QA per day
    * Scaled team up to 6
    * Not crunching
    * Many languages, many platforms
* Devops
    * Operating principles
    * Faster deployment
    * High stability
    * Better communication
    * Relationship between development and operations (deployment and management of software)
* The three ways
    * Lens on your work
    * (1) managing flow of work
    * (2) amplifying feedback loops
    * (3) continuous learning
* Managing flow of work
    * Development, operations, customer
    * Work flows in one direction
    * Eliminate waste
    * Make work visible
    * Deliver work in small batches
    * Prevent defects from moving downstream
    * Align everything toward global goals
* Eliminating waste
    * waste: anything you do that isn’t delivering value to customer “not making games”
    * Waste is always worse than you think
* The circle of waste
    * Motion: waste produced by the movement of materials or information. Better: documentation that is self service
    * Task switching: changing between contexts. Batching your work.
    * Defects: something can’t be used by downstream customer
    * Waiting: when something is supposed to happen, but doesn’t. Deliver work in small batches.
    * Unfinished projects: work on large feature that hasn’t been merged. Context of rest of the world changes. Small batch delivery.
    * Manual process: automate it.
    * Extra process: things that you don’t need to do. can we not?
    * Extra feature: something that isn’t adding to player experience
    * Do I need tiles?
    * Heroics: when unreasonable acts are required to deliver a required result. Creates every kind of waste. Signature of the game industry
    * Heroics signal that all of your systems have failed.
* Stop production. It’s the only way to break the loop.
* Making the work visible (Notion board)
    * Trello rules and production meetings
    * Twice weekly production meetings to settle on high level goals, and allocate work to meet those goals
    * “Inbox, todo, doing, testing, done
    * New tasks go into inbox and are evaluated next meeting. Avoids being derailed by unplanned work.
    * 2 day sprints
    * Time is a csontraint, not a flexible resource. Avoids burnout and crunch.
    * Work goes through the whole flow. Testing requires that everything be verified before going downstream.
    * Defects flow backwards for rework
        * Create asset, export asset, review asset ***, fix errors, update processes, export asset.
* Bottleneck in workflow
    * Process that receives more work than it can handle.
    * That’s me
    * Sam: 3 assets per hour
    * Seth: 1 asset per hour
    * What goes into game: 1 asset per hour
    * Bottleneck is Seth, but Seth task has been moved to sam, and pace of art has been increased
    * Increase the capacity of the bottleneck
* Bottleneck in deployments
    * Getting the game into people’s hands
    * If a process is painful, do it more to pave the road over
    * goal: continuous deployments
    * Constant stream of tiny changes
    * Detect problems immediately and fix them immediately
    * Fewer catastrophic failures
    * Easier to identify where problems emerge
    * Quickly fix issues with deployments
    * programmer: implement changes, write patch notes, create weekly builds, send builds to QA testers, QA team: create checklists, test changes, report issues, review issues, convert to trello cards, fix it, one week loop
    * Another 30 to 60 minutes to deploy to
    * GamePipe is born: start simple and start using immediately
        * Git push o trigger build, build uploads to dropbox
        * Game programmer time no longer compiling builds
        * No manual work of delivering builds to testers, saving time and reducing task switching and defects
        * Environment config is not a problem
        * Weekly builds become daily builds
        * Daily isn’t continuous
    * Manual: write patch notes
        * Git commits become patch notes
        * Continuous deployments, deploy at any time
        * Removes defects, like missing changes in patch notes
        * Git commits become cleaner, more readable, and more useful
    * Build deploys auto to steam
        * Build deploys to all platform
        * Automatic localization in build
        * Fully manual 1-hour process into 5 seconds
        * Weekly testing to continuous testing
        * Builds become more stable
        * Deployments are painless and easy
        * Create something simple, then improve it over time
* Next bottleneck: business administration
    * First hire since studio collapsed
    * Employee training process:
        * Inbox
        * Todo
        * Doing (sprint)
        * Testing
        * Done
    * Populated the todo list with training tasks
    * Generate knowledge and insight about her role
    * Twice weekly production meetings
    * Break tasks down by hours
    * Later used the same process to hire a full time QA
    * Make work visible
    * result: reduced strain on production, increased studio output
* First way: systems thinking
    * Development -> operations -> customer
    * Core tools: eliminate waste, make work visible: production meetings, Trello, process changes
    * Deliver work in small batches: GamePipe
    * Prevent defects from moving downstream: test at the source (test column)
    * Align everything toward global goals: relieve bottleneck pressure, one way flow faster
* Second way: amplifying feedback loops
    * Feedback allows us to catch problems, improve process, and build quality into pipeline
    * Develop tools and systems to gather feedback from people downstream
    * QA process gave continuous feedback
    * Deployment and QA testing pipeline
        * Convert to Trello card process is manual
        * Trello API to make it, add to Trello button
        * Auto trello card creation
    * Amplify how QA testers deliver feedback
        * Automated checklist creation from the patch notes
        * Turn patch notes into QA checklist
        * When I log in as a developer, devs can see number of testers who’ve tested the change
    * Develop tools and systems to gather feedback from those downstream
    * Catch problems, improve processes, build quality into pipeline
    * Have systems in place for handling feedback
* Third way: continuous learning
    * Adapt and improve and grow
    * Ensure everyone on the team has the right to experiment
    * Culture of psychological safety
    * Work culture is a result of org structure (all kinds of structure) and process
    * What structure to reinforce learning?
        * Formalized Quarterly Review
        * Fill out questionnaire
        * Use these answers plus waste analysis to look for ways to improve our processes
    * Routine Evaluation Structures Matter
        * Use them to create a culture of learning
        * Structured ways to make improvements to every process of the company
    * Evaluation doesn’t happen, improvements don’t happen
* Levelhead launch plan, June 2019
    * Nintendo announces Mario maker 2
    * Beat Mario Maker to launch?
    * Only available date is April 18, 2 months earlier than planned
    * Target: Steam
    * March 1: Pre-Alpha
    * March 8: alpha test
    * April 18: launch into early access
    * Launch in 2 weeks instead of 3 months
    * Builds were already stable and easily patchable
    * In two weeks, alpha starts
    * No major problems
    * Thousands of hours of testing: one crash. Fixed, tested, deployed within hours.
    * Early access launch day
    * No game-breaking issues.
* These days
    * Still doing continuous deployments
    * 97% positive on Steam
    * 2-3 content patches delivered to players per month
    * Patches are no big deal
    * No heroics, even with 6 platforms and 11 languages with a team of 6
    * Break the loop of heroics
    * Does it have to be like this?
* You can’t afford not to do this
    * Useful books: DevOps handbook, phonex project
    * Three ways: manage flow of work, amplify feedback loops, continuous learning
    * Takeaways:
        * Make work visible
        * Waste is worse than you think
        * Focus effort on bottlenecks
        * Focus on small batch delivery: large PRs create waste
        * Use continuous deployments to improve quality, and get feedback faster
    * Types of waste:
        * Motion
        * Task switching
        * Defects
        * Waiting
        * Manual process
        * Extra process
        * Extra features
        * Unfinished projects
        * Heroics
    * Other sources
        * The three ways: principles underlying devops by Gene Kim
        * Implementing lean software development
        * Theory of constraints
