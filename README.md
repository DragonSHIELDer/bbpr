Title: Exploring the Evolution of Vulnerability Marketplaces: Regulated, Gray and Black Markets
Abstract
The vulnerability trade has been going on for as long as computer exploits have existed.  From the business model to the organizational structure, the vulnerability market has many similarities with the traditional market. This means that research on the vulnerability market is valuable in the fields of economics, cybersecurity and cybercriminology. Here, I present a multi-phase study to investigate the market related to vulnerability, with the aim of improving the understanding of different markets and providing a comprehensive overview of the evolution of such markets. The different phases of this work are as follows:
1)Co-design study and investigation of vulnerability disclosure in ML ecosystem;
2)Large-scale measurement and cross-community study of underground exploit forums; 
3)Delphi study and comparative analysis of trust mechanism in vulnerability market.
I. Introduction
Since the development of the vulnerability market, it can be divided into various types, including legitimate (such as company-sponsored bounty programs) , black and gray markets. Figure 1 indicates the number of 0-day vulnerabilities released by CVE in recent years [1], as the number grows, the research on the white market becomes more and more important. The bug bounty program (BBP) is the representative of a legitimate market, offered by many intermediary websites, organizations, and software developers. Through the program, white hat hackers can earn reputation and rewards for reporting security vulnerabilities and bugs [2], works on BBP are beneficial to platforms, suppliers and users [3, 4]. Black markets are where 0-day exploits are traded, understanding how they work is critical to helping law enforcement effectively intervene in underground forums [5]. Exploit brokers are in a gray area [6], related work could help researchers better understand how middlemen price and trade. Previous work provided interesting research directions and critical insights about the vulnerability market, which is the motivation to conduct this research. 
In order to analyze different markets, my proposal can be divided into three phases. The object of the first phase is response mechanisms for machine learning vulnerabilities, an investigation will be conducted, including an policy analysis and an interview with security experts and ML developers, which aims to get new findings about the consensus on the definition of vulnerabilities and disclosure specifications. The second phase will be a study targeting the black market, different vulnerability underground forums will be measured, a dataset will be created and analyzed across communities. In Phase III, the comparative study of trust in vulnerability markets will build on the work of the previous two phases. An interdisciplinary Delphi survey on trust measurement in vulnerability markets will be conducted, and different markets will be analyzed comparatively.
II. Research Aim and Question
The purpose of this proposal is to explore the development and evolution of vulnerability markets, fill the gaps in previous studies. I will study such markets by focusing on investigating the following research questions through a three-phase plan: 
1)RQ1: With the rapid development and application of machine learning, how should traditional vulnerability disclosure be adapted to ML algorithms and systems?
2)RQ2: There are not many measurement studies on vulnerability trading in black markets, and datasets are also outdated, what is the status quo?
3)RQ3: Different vulnerability markets have different trust mechanisms for trading, what are the determinants affecting trust in markets?
III. Phase I A Co-Design Study of Coordination Vulnerability Disclosure in Machine Learning Ecosystem: Investigating from Security Expert and ML Developer Perspectives
3.1 Background and Related Work
More and more hackers are using machine learning technology for automatic vulnerability mining in order to obtain rewards, but machine learning-related bug bounty programs are not yet mature. As AI technologies rapidly scale and deploy across enterprises, so do their attack surfaces [7]. Twitter and Hackerone released the first algorithmic bias bounty project in 2021, the Algorithmic Justice Coalition [8] explored the feasibility of using BBPs to address algorithmic bias and the possibility of creating an algorithmic harm reporting platform similar to BBPs. Grotto et al.[9] argue that ML systems are vulnerable to a unique set of attacks that either target critical resources or exploit properties of the learning process, and may also be vulnerable to various traditional vulnerabilities. Additionally, they suggest that AI models are software programs, should be subject to vulnerability research, disclosure and management.The authors of [10] explore the possibility of assigning CVE-IDs to machine learning vulnerabilities and illustrate the changes it would cause to the current vulnerability management paradigm, but only as a thought experiment. 
Boucher et al.[11] show that after a NLP vulnerability was notified to companies and organizations, a year later these vulnerable systems are still being deployed at scale for a variety of tasks. The emerging AI industry's attitude towards vulnerabilities is very similar to that of IT companies 20 years ago, with rapid development as the first priority rather than security. The security community and the machine learning community may blame each other, just as IT companies have previously blamed white hat hackers [12].
A common vulnerability disclosure specification for the ecosystem will help resolve emerging vulnerabilities faster, which is also responsible for the security of users [13]. Therefore, it is necessary to establish a consensus on the definition of vulnerabilities and improve vulnerability disclosure specifications between the ML community and the security community. This research will conduct a collaborative design, inviting ML developers and security analysts to jointly develop the specifications.
3.2 Data Collection & Disclosure Policy Analysis
While analogs exist in the ML industry related to traditional vulnerability discovery and disclosure, the types of vulnerabilities are often fundamentally different. I will summarize the current status of some ML vulnerabilities in recent years based on the literature, and investigate the vulnerability feedback and disclosure policies in the ML industry by sampling relevant vulnerability submission specifications in AI companies to understand the status and impact. Figure 2 shows part of the content that needs to be collected.
3.3 Questionnaire & (Semi-)Structured Interview
I aimed to understand the perceptions of developers and security professionals on the definition and disclosure of vulnerabilities in this emerging technology, and to consider and address these risks such as mutual support, and build trust through training, information sharing. I will use Likert scales to analyze their attitudes, participants of different races and genders will be used to randomize and minimize interviewer bias. 
Candidate recruiting on different forums (specific to ML developers or dense developer communities) will be posted. I will describe the motivation for the project, then ask them to take part in the survey. Trace ethnography [14] will be used during the collaborative design process to analyze the process.
I am going to work with candidates to explore the trade-offs associated with ML vulnerabilities across programs and platforms, determine both parties’ concerns about target organizations, rewards, degree of disclosure (delayed/full disclosure, coordinated disclosure, non-disclosure), degree of participation (public, invitation-only/optional), project management, duration, scope and access. By summarizing the findings, it is hoped that both communities will reach a shared definition of a vulnerability, form a consensus on disclosure, and foster a diverse and inclusive community.
3.4 Expected Deliverable
1)Conduct a survey and analysis of existing ML vulnerability disclosure policies.
2)Obtain the views of ML developers and security experts on disclosure norms, provide results of the investigation.
IV. Phase II Large-scale Underground Exploit Markets Measurement
4.1 Background and Related Work
Malicious actors have built large online communities in the form of underground forums and black markets, they typically rely on these forums to trade cybercrime-related services or products [15]. The black market is relatively ano nymous, with users not disclosing their real identities and using pseudo nyms [16]. Research on various types of cybercrime and black markets has been increasing, including malware, fraudulent account, exploit and attack-as-a-service, etc [17,18]. Vulnerabilities have always been marketable in such forums, which provide a unique opportunity to learn how unregulated and illegal vulnerability markets work. Unlike vulnerability disclosure programs or bug bounty programs, researchers consider vulnerability sellers can maximize their monetary incentives in underground exploit forums [19,20]. Due to the availability of data, the vulnerability market research is mostly focused on white and gray markets, but previous work still shows many insights related to black markets [21], the study [22] discussed regulation-related implications and ethical issues in 0-day markets. Radianti et al. conducted expert interviews and literature tracking and considered that time and confidentiality are the main factors affecting black market supply and demand behavior [23], they also built a system dynamics model and analyzed potential factors affecting the emergence of a black market for vulnerabilities [24], then discussed the salient features of internal actors, interactions, and mechanisms [25]. A study conducted by Luca [26] analyzed data from the Russian forum RuMarket, the author cites the vulnerability price and severity as factors that may affect the probability of finding vulnerabilities at scale, but this result is limited to RuMarket. 
It can be found that there is no such cross-market quantitative work on vulnerabilities in recent years, and no such new datasets have been provided. Therefore, a measurement of the underground exploit market is necessary. Forum markets provide valuable information about the state of the underground economy [27], and large-scale analysis of these monetization structures is critical to understanding the motivations and interests of forum members. This study will measure the vulnerability black markets of the forums in different languages, including the current scale of transactions, with a focus on the business model. In addition, this study will also help law enforcement officers to effectively intervene in related illegal markets.
4.2 Data Source Selection & Collection
This research focuses on English and Russian underground markets. Due to the short lifetimes of online black markets [35], some of the above data sources may be outdated. Potential data sources determined from related work and reports are shown in Table 1[28,29,30], and new markets will be identified.
Ethical issues need to be considered first[31], I plan to consult with the Research Ethics Board and law enforcement agencies before the start of this cybercrime research. Data collection should not scrape any personal information. The crawler shown in Figure 3 used for data collection in this research can be customized based on the general-purpose crawler models and modules.
4.3 Cross-Community Analysis
After the establishment of the large-scale dataset, market characteristics will be compared. Economic indicators related to price levels, sellers and market access conditions will be analyzed to describe business models of vulnerability black markets.
4.4 Expected Deliverable
1)Identify underground marketplaces currently providing exploit trading, and develop a multi- source crawler.
2)Establish an available and reproducible dataset of underground exploits forums.
3)Show the current situation of black markets, including business models and transaction status of 0-day and N-day vulnerabilities.
V. Phase III How to Build Trust in Vulnerability Markets: A Comparative Study
5.1 Background
After the first two phases of the research, a deeper understanding will be had of how to research the whole vulnerability market ecosystem. As illustrated in Figure 4, the vulnerability market can be divided into three categories [32]. For white and black markets, the previous two chapters have introduced related research. For the gray market, Dellago et al. [33] recently conducted research on prices and transactions of exploit brokers and provided empirical insights. For the entire vulnerability market, Armin et al. [34] compared different exploit markets from an arms control perspective, arguing that market forces and cybercriminal activities drive research on 0-day exploits. Allodi et al. [35] quantified the strong correlation between market activity and the likelihood of exploitation, and showed that black market prices are often in line with or higher than the legal market’s. 
The common feature of different vulnerability markets is information asymmetry [36], for markets to work, trust must be built first, when one party pays for a vulnerability, they can ensure that the other side of the transaction is supported. Without a trust mechanism, these markets would collapse. There is currently no comparative study of trust mechanisms in the three markets, and it is the motivation for this work. My study plans to determine the trust factor and establish a measurement framework in the market through a Delphi study and a comparative analysis. The Delphi method is typically used to gather and determine expert opinions on a particular topic. Del-Real et al. [37] analyzed the possibility of ethical hacking patterns of behavior under supervision through the Delphi approach, including bug bounty programs and coordinated vulnerability disclosure policies. 
5.2 Systematic Literature Review
A systematic literature review of economics and trade-related studies about vulnerability marketplaces will be implemented first. I will conduct a search by keyword using databases such as Google Scholar, Springer, ScienceDirect, ACM Library and IEEE Xplore. Results will not be limited to scholarly articles, but include journals, magazines and newspapers, the number of publications is then determined by screening.
5.3 Delphi Study
The first round of the Delphi panel will be launched, emailing the questionnaire to the experts and explaining the purpose, rules and methods of the experiment. Participants will rate their level of agreement with the determinants and influencers extracted from the literature, while also allowing them to make modifications and additions based on their extensive knowledge of the topic. After improving the questionnaire, the second and third rounds of surveys will be conducted to reach a consensus among the experts. Finally, a framework for measuring trust in the exploit market will be proposed.
5.4 Comparative Analysis
Three markets of different types will be selected as cases, and a comparative study will be conducted. I will compare the trust mechanisms of BBPs, exploit brokers and underground markets, then analyze their trust-building process.
5.5 Expected Deliverable
1)Conduct a literature review of all studies surrounding vulnerability marketplaces, with a focus on trust and business-related work.
2)Propose a framework for measuring trust in vulnerability markets through the survey.
3)Provide interdisciplinary insights into the evolution of trust mechanisms in vulnerability markets.
VI. Conclusion
The first phase of my research is an investigation of vulnerability disclosure standards for the machine learning industry, including a policy analysis an interview with developers and security analysts. The second phase will be a measurement targeting black markets, different underground forums will be compared, a dataset will be created and analyzed across communities. In Phase III, an interdisciplinary Delphi survey on trust measurement in vulnerability markets will be conducted, and different markets will be analyzed comparatively. I envisage that this research can improve CVD’ performance, strengthen law enforcement in underground exploit markets, and provide researchers with a comprehensive overview of the evolution of vulnerability markets.
