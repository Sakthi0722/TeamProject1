# *Continuous Integration*

![continuous_integration](https://i.ytimg.com/vi/JmH4qKeQ6ro/maxresdefault.jpg)


**Continuous integration (CI)** is the practice of automating the integration of code changes from multiple contributors into a single software project. The CI process is comprised of automatic tools that assert the new code’s correctness before integration. A source code version control system is the crux of the CI process. The version control system is also supplemented with other checks like automated code quality tests, syntax style review tools, and more.

## *What CI does*

**CI helps to scale up headcount and delivery output of engineering teams.** Introducing CI to the aforementioned scenario allows software developers to work independently on features in parallel. When they are ready to merge these features into the end product, they can do so independently and rapidly. CI is a valuable and well-established practice in modern, high performance software engineering organizations.

## *How CI can be used*

**CI is generally used alongside an agile software development workflow.** An organization will compile list of tasks that comprise a product roadmap. These tasks are then distributed amongst software engineering team members for delivery. Using CI, enables these software development tasks to be developed independently and in parallel amongst the assigned developers. Once one of these tasks is complete, a developer will introduce that new work to the CI system to be integrated with the rest of the project.

## *CI vs Continuous Deployment vs Continuous Delivery*

**Continuous integration, deployment, and delivery are three phases of an automated software release pipeline. These three phases take software from idea to delivery to the end user.** The integration phase is the the first step in the process. Integration covers the process of multiple developers attempting to merge their code changes with the master code repository of a project.

**Continuous Delivery is the next extension of continuous integration.** The delivery phase is responsible for packaging an artifact together to be delivered to end users. This phase runs automated building tools to generate this artifact.

**Continuous Deployment is the final phase of the pipeline.** The deployment phase is responsible for automatically launching and distributing the software artifact to end users. At deployment time, the artifact has successfully passed the integration and delivery phases. Now it is time to automatically deploy or distribute the artifact.


# *Benefits and challenges of Continuous Integration (CI)*

CI is a valuable asset to a software producing organization. **CI benefits are not limited to the engineering team but greatly benefit the overall organization.** CI enables better transparency and insight into the process of software development and delivery. These benefits enable the rest of the organization to better plan and execute go to market strategies. The following are some of the overall organizational benefits of CI.

## *1. Enable Scaling*

CI enables organizations to scale in engineering team size, codebase size, and infrastructure. By minimizing code integration bureaucracy and communication overhead, CI enhances agile workflows. It allows each team member to own a new code change set through to release. CI enables scaling by removing any organizational dependencies between development of individual features.

## *2. Improve the feedback loop*

Faster feedback on business decisions is another advantage of CI. Product teams can test ideas and iterate product designs faster with an optimized CI platform. Changes can be rapidly pushed and measured for success. Bugs or other issues can be quickly addressed and repaired.

## *3. Enhance Communication*

By introducing pull request work flows tied to CI, developers gain passive knowledge share. Developers can now view and collaborate on feature branches with other developers as the features progress through the CI Pipeline. An efficient CI pipeline with high-confidence automated test coverage will safeguard from regressions and ensure that new features match a specification. Before new code is merged it must pass the CI test assertion suite which will prevent any new regressions.

>Adding to that, the real challenges of CI arise when transitioning a project form no CI to CI. Most modern software projects will adopt CI from early inception stages and alleviate the challenges of later adoption.

## *4. Adoption and installation*
  
The challenges of continuous integration are primarily around team adoption and initial technical installation. If a team doesn't currently have a CI solution in place, it can require some effort to pick one and get started. Thus, considerations need to be made around the existing engineering infrastructure when installing a CI pipeline.

## *5. Technology learning curve*

CI functionality comes with a list of supportive technologies that may be learning curve investments for the team to undertake. These technologies are version control systems, hosting infrastructure, and orchestration technologies.


# *CI Best Practices*

*1. Test Driven Development*

*2. Pull requests and code review*

*3. Optimize pipeline speed*


# *Summary*

*CI is a standard fixture of modern high efficiency software development organizations. The best companies have robust CI pipelines and don’t think twice about further efficiency investments. The benefits of CI are not limited to the engineering team and applicable to the whole organization.*