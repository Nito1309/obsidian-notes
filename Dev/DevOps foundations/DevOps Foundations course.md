

Course link: [DevOps Foundations](https://www.linkedin.com/learning-login/share?account=2101329&forceAccount=false&redirect=https%3A%2F%2Fwww.linkedin.com%2Flearning%2Fdevops-foundations-23454205%3Ftrk%3Dshare_ent_url%26shareId%3DUGpIFHqsQACsa%252BBXJzQk2w%253D%253D)

1. CAMS model
	* Culture
		* Mutual understanding 
		*  Different work ways
		* Paradigms
	* Automation
		* You don't have to invert all your time in this point
		* Create and control your systems
		* Accelerator to help you unlock other DevOps benefits
	* Measurement
		* What is happening?
		* Did changes improve things? (Key measurements).
	* Sharing
		* Documentation
		* Pair programming
		* Reviews
		* Mentoring
2. The three ways
	1. Systems thinking and the principles of flow.
		* Do not try to optimize a part but at the end it costs more time in a big view.
		* Focus on the overall outcome 
		* Understand the whole system to optimize it
	2.  Amplifying feedback loops. 
		* Feedback loop is a process that takes its own output into consideration when deciding what to do next
		* Prevents a bug was discovered by a client and all the time to fix it.
		* They must be short and effective
	3. A culture or continuous experimentation and learning.
		* Create team processes and standards
		* Encourage sharing and trying new ideas
3. DevOps playbook
	* Culture
		* Safe environment
		* Communication
		* Collaboration
		* Change mindset how people work
	* Process 
		* Learn, share, experiment
	* Infrastructure as code 
		* Use cloud, containers to create software
	* Continuous delivery
		* Automation to implement lean principles, 
		* Test and deploy software with small changes
	* Site reliability
		* Apply engineering to achieve reliability in the application
4. Tools
	*People over process over tools* - Alex Honors

	* Who is responsible for a job function, skills and support. Then...
	* Define the process that needs to happen. Then...
	* Select and implement the tools to achieve the process.
	* Choose criteria
		* How does the tool make everyone collaborate together?
		* KISS -> Keep it simple, stupid
		* DevOps toolchain
		* Adapt to change
5. Break down team barriers (wall of confusion)
	* Cross functional teams
	* Alignment goals
	* Use self-service tooling
	* Plan - Do - Check - Act
	* Critical thinking
	* Gemba / Kaizen
		* emphasizes going right to the source where value is being created
6. DevOps is an extension of agile
7. Lean Remove waste *muda* (unnecessary, necessary but no value...)
8. Change control
	* Review
		 Every change needs to be reviewed, approved and documented.
	* Lightweight
		 Changes should be kept as small as possible
	* Test
		 All changes should be tested
	* Schedule
9. Infrastructure as code
	* Provisioning and managing infrastructure through writing automation code
	* Write code in version control system
	* Run it through a build system that tests it
	* End up with a single artifact that can be downloaded
	* Configuration management
		 Process to create and maintain computer systems and software in a desired, consistent state.
		 1. Provisioning
		     Creating a system of computing infrastructure and making it ready for operation
		 2. Deployment
		     Installing and upgrading applications on a system
		 3. Orchestration
		     Performing coordination and management of computer systems and software
		     ![[Pasted image 20240814141913.png]]
10. CI / CD
  ![[Pasted image 20240814202639.png]]
	* CI (Continuous Integration): Automatically build and test each code change
	* CD (Continuous Delivery): Automatically deploy and test each code change
	* Continuous Deployment: Automatically release each passing release candidate to production
12. Six CI practices
	1. Fast builds
	2. Commit small changes
	3. Don't leave the build broken
	4. use a trunk-based development flow
	5. don't allow flaky automated test, fix it
	6. the build should return a status, a log or an artifact
13. Five CD practices
     *it's now how much you can deliver, but how little*
    1. Build artifacts only once
    2. Artifact should be immutable
    3. Deploy to a production-like environment
    4. Stop deploys if a previous step fails
    5. Deploys should be idempotent (ensures that if the operation is repeated more than once you get the same result).
13. Testing 
	* Unit testing
	* Code hygiene
	* Integration testing
	* Acceptance (end-to-end) testing
	* TDD (test driven dev) / BDD (behavior driven dev)
		 Test the app before the implementation and after it, and compare the changes.
	* Three Strategies
		1. Run non-blocking test in parallel in your pipeline.
		2. Use scheduled testing (for example, nightly test suite)
		3. Run them continuously

 