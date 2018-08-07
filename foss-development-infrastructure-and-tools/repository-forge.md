# Repository/Forge

## Repository/Forge

In open source software development, a repository is a file archive and web hosting facility where a large amount of source code and project meta data is kept, either publicly or privately. A repository is often used for multi-developer cooperation and software version controls. Repositories help developers submit patches of code in an organized fashion.

[Version Control Repository - Wikipedia](https://en.wikipedia.org/wiki/Repository_%28version_control%29) 

[Comparison of source code hosting](https://en.wikipedia.org/wiki/Comparison_of_source_code_hosting_facilities)

### Types and management of repository

Each revision control system handles storing changes differently. Traditionally, subversions are stored into databases. Nowadays, solutions directly on the filesystem or on the cloud is becoming more common.

Depending on the version control system, whether it is centralized or distributed, the whole set of information in the repository may be duplicated on every user's system or may be maintained on a single server.

### Components of repository

Some of the metadata that a repository contains includes, among other things:

* A historical record of changes in the repository. 
* A set of commit objects. 
* A set of references to commit objects, called heads.

### Features to consider when choosing software repository

* What functionality do you need now?
* Access Control \(e.g. setting up project level roles\)
* How easy is it to upgrade to additional functionality in the future? 
* What is your preferred version-control system, e.g. CVS, SVN, Git, Mercurial? 
* Is it important to have your code publicly available?
* Are all your code committers local? 
* How easy is it to integrate other things you run separately \(e.g. a website\) with the repository? 
* How good is the support for your IDEs of choice? 
* Is there support for authentication systems such as OpenID or SSH keys? 
* What additional forge, social networking, project-management functionality do you want from the site? e.g. GitHub is good for social coolness 
* Where are similar projects to yours hosted? 
* What's the speed of upload/download? 
* How easy is it to backup the entire repository \(code, mailing lists, issue tickets, ...\) 
* How established and stable is the repository? 
* How good is the user support? 
* How much effort do you have to put into repository maintenance? 
* Would it be better to use more than one repository, e.g. code stored in GitHub and a link to Assembla for its extra tools? 
* What are the Service Level Agreements for uptime, downtime, time to fix outages and bandwidth?

[Reference](https://www.software.ac.uk/resources/guides/choosing-repository-your-software-project)

### Examples of repository web hosting service

The interfaces of an online repository often appears to be a webpage, where there are version control \(including online code viewing\), bug/issue tracking, release management, mailing lists, statistics reporting \(e.g. number of commits, number of downloads\) and wikibased documentation.

Project/release managementThere are many repository web hosting services, such as

* Github 
* BitBucket 
* Cloud Forge 
* Source forge 
* Launchpad 
* Assembla 
* Codeplex 
* Freepository 
* Codebase 
* ProjectLocker

### Example case study

#### Github

[GitHub ](https://github.com/)  
[GitHub - Wikipedia](https://en.wikipedia.org/wiki/GitHub)

GitHub is a web-based Git or version control repository and Internet hosting service. It offers all of the distributed version control and source code management \(SCM\) functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.

Any user could register a github account and then create his own project repository. The repository could be either private or public. Usually, the repository is licensed with a particular license \(LISENSE.TXT/LICENSE\) and an introduction file \(README/README.md\).

Using the git version control system, a user could create his local repository on his machine, add files and commit to it. With github repository, the user could push/pull changes in the remote repository and keep the file changes synchronized between local and the cloud.

### Bitbucket

{% embed data="{\"url\":\"https://bitbucket.org/\",\"type\":\"link\",\"title\":\"Bitbucket \| The Git solution for professional teams\",\"description\":\"Collaborate on code with inline comments and pull requests. Manage and share your Git repositories to build and ship software, as a team.\",\"icon\":{\"type\":\"icon\",\"url\":\"https://bitbucket-marketing-cdn.atlassian.com/assets/img/favicons/bitbucket/apple-touch-icon.png\",\"width\":180,\"height\":180,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://bitbucket-marketing-cdn.atlassian.com/dam/jcr:1437c132-1dbc-410d-b6a6-cb7fce8f2775/Bitbucket@2x-blue.png\",\"width\":888,\"height\":128,\"aspectRatio\":0.14414414414414414}}" %}

{% embed data="{\"url\":\"https://en.wikipedia.org/wiki/Bitbucket\",\"type\":\"link\",\"title\":\"Bitbucket\",\"description\":\"Bitbucket is a  web-based version control repository hosting service owned by Atlassian, for source code and development projects that use either Mercurial \(since launch\) or Git \(since October 2011&\#91;2&\#93;\) revision control systems. Bitbucket offers both commercial plans and free accounts. It offers free accounts with an unlimited number of private repositories \(which can have up to five users in the case of free accounts\) as of  September&\#160;2010&\#91;update&\#93;. Bitbucket integrates with other Atlassian software like Jira, HipChat, Confluence and Bamboo.\\n\",\"icon\":{\"type\":\"icon\",\"url\":\"https://en.wikipedia.org/static/apple-touch/wikipedia.png\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"//upload.wikimedia.org/wikipedia/en/thumb/d/df/BitBucket\_SVG\_Logo.svg/250px-BitBucket\_SVG\_Logo.svg.png\",\"width\":250,\"height\":63,\"aspectRatio\":0.252}}" %}

Bitbucket is a web-based hosting service for source code and development projects that use either Mercurial \(since launch\) or Git \(since October 2011\[2\]\) revision control systems that is owned by Atlassian. Bitbucket offers both commercial plans and free accounts. It offers free accounts with an unlimited number of private repositories \(which can have up to five users in the case of free accounts\) as of September 2010. Bitbucket integrates with other Atlassian software like JIRA Software, HipChat, Confluence and Bamboo.

It is similar to GitHub, which primarily uses Git. Bitbucket has traditionally tailored itself towards helping professional developers with private proprietary code, especially since being acquired by Atlassian in 2010. \[3\] In September 2016, Bitbucket announced it had reached 5 million developers and 900,000 teams on its platform. \[4\] Bitbucket has 3 deployment models: Cloud, Bitbucket Server and Data Center.

### Source Forge

[SourceForge](https://sourceforge.net/)  
[SourceForge - Wikipedia](https://en.wikipedia.org/wiki/SourceForge)

SourceForge is a Web-based service that offers software developers a centralized online location to control and manage free and open source software projects. It provides a source code repository. Users can create their projects on sourceforge easily.

### Cloud Forge

{% embed data="{\"url\":\"http://www.cloudforge.com/\",\"type\":\"link\",\"title\":\"Free Subversion and Git Hosting \| Bug and Issue tracking \| CloudForge\",\"description\":\"Unlimited Users, Unlimited Projects for FREE! CloudForge delivers Agile tools and services for developing and deploying in the C\",\"icon\":{\"type\":\"icon\",\"url\":\"http://www.cloudforge.com/favicon.ico\",\"aspectRatio\":0}}" %}

{% embed data="{\"url\":\"https://en.wikipedia.org/wiki/CloudForge\",\"type\":\"link\",\"title\":\"CloudForge\",\"description\":\"CloudForge is a software-as-a-service product for application development tools and services, such as Git hosting, Subversion \(SVN\) hosting, issue trackers and Application Lifecycle Management. CloudForge was built on CollabNet’s cloud hosting and integration platform, acquired from Codesion.com in October 2010.&\#91;1&\#93;\\n\",\"icon\":{\"type\":\"icon\",\"url\":\"https://en.wikipedia.org/static/apple-touch/wikipedia.png\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"//upload.wikimedia.org/wikipedia/en/8/8d/Cloudforge200.png\",\"width\":200,\"height\":37,\"aspectRatio\":0.185}}" %}

CloudForge is a software-as-a-service product for application development tools and services, such as Git hosting, Subversion \(SVN\) hosting, issue trackers and Application Lifecycle Management. CloudForge was built on CollabNet’s cloud hosting and integration platform

