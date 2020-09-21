# Continuous Integration

Continuous integration (CI) is the practice of automating the integration of code changes from multiple contributors into a single software project. The CI process is comprised of automatic tools that assert the new code’s correctness before integration. A source code version control system is the crux of the CI process. The version control system is also supplemented with other checks like automated code quality tests, syntax style review tools, and more.


# Importance of Continuous Integration (CI)

In order to understand the importance of CI, it’s helpful to first discuss some pain points that often arise due to the absence of CI. Without CI, developers must manually coordinate and communicate when they are contributing code to the end product. This coordination extends beyond the development teams to the rest of the organization, as well. Product teams must coordinate when to sequentially launch features and fixes and which team members will be responsible.

The communication overhead of a non-CI environment can become a complex and entangled synchronization chore, which adds unnecessary bureaucratic cost to projects. This causes slower code releases with higher rates of failure, as it requires developers to be sensitive and thoughtful towards the integrations. These risks grow exponentially as the engineering team and codebase sizes increase.

Without a robust CI pipeline a disconnect between the engineering team and the rest of the org can form. Communication between product and engineering can be cumbersome. Engineering becomes a black box which the rest of the team inputs requirements and features and maybe gets expected results back. It will make it harder for engineering to estimate time of delivery on requests because the time to integrate new changes becomes an unknown risk.

## What CI does

CI helps to scale up headcount and delivery output of engineering teams. Introducing CI to the aforementioned scenario allows software developers to work independently on features in parallel. When they are ready to merge these features into the end product, they can do so independently and rapidly. CI is a valuable and well-established practice in modern, high performance software engineering organizations.

##How CI can be used

CI is generally used alongside an agile software development workflow. An organization will compile list of tasks that comprise a product roadmap. These tasks are then distributed amongst software engineering team members for delivery. Using CI enables these software development tasks to be developed independently and in parallel amongst the assigned developers. Once one of theses tasks is complete, a developer will introduce that new work to the CI system to be integrated with the rest of the project.

## CI vs Continuous Deployment vs Continuous Delivery

Continuous integration, deployment, and delivery are three phases of an automated software release pipeline. These three phases take software from idea to delivery to the end user. The integration phase is the the first step in the process. Integration covers the process of multiple developers attempting to merge their code changes with the master code repository of a project.

Continuous Delivery is the next extension of continuous integration. The delivery phase is responsible for packaging an artifact together to be delivered to end users. This phase runs automated building tools to generate this artifact. This build phase is kept ‘green,’ which means that the artifact should be ready to deploy to users at any given time.

Continuous Deployment is the final phase of the pipeline. The deployment phase is responsible for automatically launching and distributing the software artifact to end users. At deployment time, the artifact has successfully passed the integration and delivery phases. Now it is time to automatically deploy or distribute the artifact. This will happen through scripts or tools that automatically move the artifact to public servers or to another mechanism of distribution, like an app store.


# Benefits and challenges of Continuous Integration (CI)

CI is a valuable asset to a software producing organization. CI benefits are not limited to the engineering team but greatly benefit the overall organization. CI enables better transparency and insight into the process of software development and delivery. These benefits enable the rest of the organization to better plan and execute go to market strategies. The following are some of the overall organizational benefits of CI.

## 1. Enable Scaling

CI enables organizations to scale in engineering team size, codebase size, and infrastructure. By minimizing code integration bureaucracy and communication overhead, CI enhances agile workflows. It allows each team member to own a new code change set through to release. CI enables scaling by removing any organizational dependencies between development of individual features. Developers can now work on features in an isolated silo and have assurances that their code will seamlessly integrate with the rest of the codebase.

## 2. Improve the feedback loop

Faster feedback on business decisions is another powerful side effect of CI. Product teams can test ideas and iterate product designs faster with an optimized CI platform. Changes can be rapidly pushed and measured for success. Bugs or other issues can be quickly addressed and repaired.

## 3. Enhance Communication

Overall engineering communication and accountability is improved with CI. By introducing pull request work flows tied to CI, developers gain passive knowledge share. Pull Requests allow Developers to observe and comment on code from other team members. Developers can now view and collaborate on feature branches with other developers as the features progress through the CI Pipeline. CI can also be used to help QA resource expense. An efficient CI pipeline with high-confidence automated test coverage will safeguard from regressions and ensure that new features match a specification. Before new code is merged it must pass the CI test assertion suite which will prevent any new regressions.

The benefits of CI far outweigh any challenges in adoption. That said, it is important to be aware of the challenges of CI. The real challenges of CI arise when transitioning a project form no CI to CI. Most modern software projects will adopt CI from early inception stages and alleviate the challenges of later adoption.

## 4. Adoption and installation
  
The challenges of continuous integration are primarily around team adoption and initial technical installation. If a team doesn't currently have a CI solution in place, it can require some effort to pick one and get started. Thus, considerations need to be made around the existing engineering infrastructure when installing a CI pipeline.

## 5. Technology learning curve

CI functionality comes with a list of supportive technologies that may be learning curve investments for the team to undertake. These technologies are version control systems, hosting infrastructure, and orchestration technologies.


# CI Best Practices

## 1. Test Driven Development

Test Driven Development (TDD) is the practice of writing out the test code and test cases before doing any actual feature coding. Pure TDD can closely involve the product team to help craft an expected business behavior specification, which can then be transformed into the test cases. In a pure TDD scenario, developers and product team will meet and discuss a spec or list of requirements. This list of requirements will then be converted into a checklist of code assertions. The developers will then write code that matches these assertions.

## 2. Pull requests and code review

Pull requests are an opportune time to kick off the CI pipeline and run the set of automated approval steps. An additional, manual approval step is commonly added at pull request time, during which a non-stakeholder engineer performs a code review of the feature.. This allows for a fresh set of eyes to review the new code and functionality. The non-stakeholder will make edit suggestions and approve or deny the pull request.

Pull requests and code review are a powerful tool to foster passive communication and knowledge share among an engineering team. This helps guard against technical debt in the form of knowledge silos, where specific engineers are the only stakeholders for certain features of a code base.

## 3. Optimize pipeline speed

A faster CI pipeline enables a faster product feedback loop. Developers can rapidly push changes and experiment with new feature ideas to help improve the user experience. Any bug fixes can be quickly patched and resolved as discovered. This increased execution speed can offer both an advantage over other competitors and an overall higher-quality experience to your customers.


# Summary

CI is a standard fixture of modern high efficiency software development organizations. The best companies have robust CI pipelines and don’t think twice about further efficiency investments. The benefits of CI are not limited to the engineering team and applicable to the whole organization.

Many 3rd party tools exist to aid in CI management and installation.There are many options to choose from. Some popular options are Codeship, Bitbucket Pipelines, SemaphoreCI, CircleCI, Jenkins, Bamboo, Teamcity and many others. These tools have their own in depth setup guides and documentation to help get started.

Bitbucket pipelines and Bamboo are great utilities to bring a project up to speed with modern CI features. Jira is one of the world's most popular agile project management tools. Jira tightly integrates with other Bitbucket projects and when coupled with a CI pipeline, can give a very transparent view into execution health of an organization.
