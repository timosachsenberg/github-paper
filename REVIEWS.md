> We would like the reviewers for their insightful comments and
> suggestions, which helped us to improve the manuscript. As a result, the revised of the manuscript has changed significantly.


# Reviewer 1

The authors provide a fairly comprehensive overview of how to use
GitHub for scientific computing projects, with some specifics about
bioinformatics.
 
First, let me say that I am a huge fan of git and github, and have no
complaints about the overall message. My only concern is to help the
authors deliver an effective argument!

That having been said, I find the organization and discussion of this
paper to be confusing and to do a somewhat poor job of "selling"
GitHub. The discussions are overcomplicated and read like a wall of
text, rather than making clear, specific points.

For example, "Rule 1".

- the title makes no sense if you don't already know something about github.
- I'm not sure what the main message is intended to be - there are several
currently - but I like the sentence starting with "Github organisations
are a great way". Perhaps "GitHub can be used for collaboration"?
- but that might be a bad introduction. Why not, "you should be using git
in the first place" (rule 2) as rule 1?

> Response: We agree with the reviewer's comments. In the current version we
> have streamlined the rules to make them more useful. At the same
> time we created an introductuty rule Rule 1 that explain the basic
> concepts behind GitHub. Also, we created a Supplemental Note
> including comments and concepts for advanced users such as continues integration, testing, etc.

I think the authors should take a step back and simplify their 10 main
messages, and then write around that. Here is an example (not well
thought out) --

Rule 1: Use GitHub to track your lab and personal proejcts.
Rule N: Use GitHub to deliver and maintain versions of your code.
Rule N: Use GitHub to advertise your project. (can include web site)
rule N: Use GitHub to track issues reported by users.
Rule N: GitHub integrated services can do lots of nice things (CI).

> Response: We have updated the rule names as follows:

```
## Rule 1. Use GitHub to track your projects
## Rule 2. GitHub for single users, teams and organizations
## Rule 3. Developing and collaborating on new features: branching and forking
## Rule 4. Naming branches and commits: tags and semantic versions
## Rule 5: Let GitHub do some tasks for you: integrate
## Rule 6: Let GitHub do more tasks for you: automate 
## Rule 7. Use GitHub to openly and collaboratively discuss, address and close issues
## Rule 8. Make your code easily citable, and cite source code!
## Rule 9. Promote and discuss your projects: web page and more
## Rule 10. Use GitHub to be social: follow and watch
```

> We now name GitHub where it provides the main feature. In contrast, we don't do it now when
> it's (mainly) a git feature. More generally, we think that the Rule titles are more engaging
> now.

I am happy to provide more detailed critiques but I think the overall
organization is getting in the way of the message.

I would also urge the authors to post this as a pre-print and get some
discussion of it going in public[*]. There are lots of academics using
github and you will get quite a bit of helpful advice.

> Response: As suggested by the reviewer, we made this discussion available under the manuscript repository (see the twitter feed https://twitter.com/lgatt0/status/715199736437989376).
> As a result, six additional authors have contributed to the manuscript. We also addressed dozens
> of new issues from contributors and refined the paper repo structure including TRAVIS, LICENSE, and
> a better deploy system. 

[*] perhaps you could use github to do this? :)

## Meso comments:

Plans that provide some private repositories are free for academic users
of github. This is one of the major concerns of adoption; might be worth
highlighting. (I think everything should be open, but that's a hard message
to swallow.)

> Response: We mention *GitHub also offers paid plans for private repositories
> for individuals and businesses, as well as free plans including
> private repository for research and educational use.* The debate
> between everything being open vs keeping (some) things close is
> certainly an important one. We have tried to highlight the
> importance of openness and open source throughout the manuscript,
> but we feel it is not the right venue for this debate.

Github large file support is not free, generally speaking.

> Response: We now discuss what is GitHub LFS in the light of project
> management and binary/text/big files in the first rule and mention
> quotas and fees (**Box 1**).

In the conclusions, the (substantial) learning curve of git is
mentioned. Perhaps some pointers to open lessons should be made
available, along with workshops? For example, both Data Carpentry and
Software Carpentry teach git and github on a global basis.
(Disclaimer: I am heavily involved with both.)

> Response: We agree with the reviewer and in the updated version, we added some
> useful links to documentation, courses and tutorials (Table 2).

## Minor comments:

It could be made clearer that all files involved in a change are made
part of a single revision.

> Response: This has been clarified as part of the improved (new) rule 1.

Gitter is not owned by github, AFAIK. They just integrate. (Line 203).
Why prioritize it over others? For example, Slack is another service
that provides similar functionality. (We use gitter, but still.)

> Response: We agree with the reviewer. In the new version we refined the
> paragraph, making it clear that Gitter is not the only chat system
> integrated with Github and mention also Slack. Gitter serves
> (amongst several alternatives) as a popular example for a Github
> integrated chat system.

Rule 10 title should be "Periodically check..."

> Response: The rule name has been updated (see above).

missing reference:
http://scfbm.biomedcentral.com/articles/10.1186/1751-0473-8-7

> Response: Thank you for this suggestion. We have added this (and other)
> references to other useful git/GitHub tutorials and introductions.

Signed,

C. Titus Brown
ctbrown@ucdavis.edu


# Reviewer 2

This paper provides valuable orientation to modern 'best practices'
for nascent developers of bioinformatic software. The manuscript will
appeal to an important part of the bioinformatics community, and will
help many individuals take the 'next step' in solidifying their
overall contribution.

1. Reproducibility should not be mentioned (in the introduction) as a
   motivating factor. Having available software is of course a
   necessary condition, but in reality the temporal scale (years after
   the original analysis) and complexity (operating systems,
   compilers, libraries, software ecosystem, ...) of analyses really
   mean that the individual investigator interested in reproducible
   research MUST take charge of the situation at the time of the
   original analysis, and cannot rely on availability of versioned
   software after the fact.
   
> Response: Indeed, reproducibility is a broader issue that software alone will not
> solve. We replaced the word reproducibility by two different terms:
> replicability and traceability. The current version of the
> manuscript explains: "To enable and ensure the
> replicability and traceability of scientific claims, it is essential
> that the scientific publication, the corresponding datasets, and the
> data analysis are made publicly available \cite{Goodman:2014,Perez-Riverol:2015}."

2. It would be very helpful to call out, with links to repository
   locations, exemplar GitHub repositories of individual developers
   (from among the authors?), labs (from the authors, or from
   successful projects / groups like bedtools, Lior Pachter's lab?),
   intermediate projects (hts / samtools?), and larger projects
   (rOpenSci??) that effectively use GitHub.
   
> Response: We now discuss exemplar repositories in the introduction. We added a complete table with examples 
> of GitHub projects organized by categories (Table 1). Each example can be used as a reference for each Rule in the paper.
> For all the examples, the name, URL and specific categories are added to the table."

3. Of course the emphasis on GitHub is challenging. We know that this
   service cannot be indefinite, just as Sourceforge, Google Code,
   etc., have all faded. The manuscript should emphasize principles as
   much as possible, rather than the GitHub realization of those
   principles; I realize that GitHub does a great job of bringing
   bioinformatics developers into the modern age. Minimally, I think
   that Git and GitHub should be removed from the title and all
   'Rules' headers.
   
> Response: We partially agree with the reviewer. Git is an open source project
> that is not part of GitHub, and, as such, is immune to what happened
> to Google Code. GitHub, on the other hand, is not. In the revised
> version of the manuscript we have removed GitHub from those rules where we do not
> rely on an explicit GitHub feature. However, some of the rules are
> focused on the functionalities provided by GitHub, and, in those
> cases, we keep the term.

> More generally, corporate support is a double edge sword: companies
> often produce clean products and support, but users are at the mercy
> of financially motivated decision. On the good side, thanks to the
> distributed nature of git, users would not lose their repositories
> nor the commit history. Issues could be downloaded using the GitHub
> API, but the nice interface would be lost. This is a risk that some
> might not take, and certainly a discussion worth having, albeit not
> in the manuscript.

> Response: We have highlighted this point in an issue that can be found in the manuscript
> repository (https://github.com/ypriverol/github-paper/issues/92) to
> make it more visible.

4. The merits of individual recommendations should be reinforced with
   links to relevant examples, e.g., of an open issue, relevant
   commentary, and appropriate resolution. Similarly oriented links
   would help to convey the value / ease of continuous integration,
   and of test coverage.
   
> Response: Thank you for this suggestion. In the current version of the
> manuscript we included examples in most of the sections of the
> manuscript (see Table 1).

5. The target audience is the relatively 'novice' developer; more
   established researchers will have their own procedures in place,
   will be aware of the current state-of-the-art, or will be too stuck
   in their ways to benefit from the discussion. From this
   perspective, it seems counter-productive to include 'organizations'
   and even 'teams' in rule 1; really one wants to get the individual
   or at most the individual + lab group oriented; 'organizations'
   (including the GitHub concept) are not immediately relevant.
   
> Response: We undestand the reviewer's point. However, we think we should
> explain most of the features of GitHub. We have added
> examples about how to use the different components and to explain in
> a better way every GitHub/git concept. In addition, we now have a
> different Rule 1, that focuses on git/GitHub basics for new users.
> More complex concepts have been added to the Suplemental Note for those readers, with a higher degree of 
> expertise. 

6. Rule 3 should be refined to emphasize that branches are really
   short-term departures from master; it is too easy for academic
   developers to lose track of the thrust of their project, or for
   individuals to work in isolation for extended periods, so that
   their contribution cannot easily be merged back to master.
   
> Response: We agree with the reviewer. The current version emphasizes the use of
> branches as short-term departures from the master branch: "When developing
> different features in parallel, there is a risk to apply
> incompatible changes in different branches/forks; these are said to
> become out of sync. Branches are just short-term departures from
> master. If you pull frequently, you will keep your copy of the repo
> up to date, and you will have the opportunity to merge your changed
> code with others' contributors without requiring to manually address
> conflicts to bring the branches in sync again."

7. Rule 5 should be clarified. It includes really two points. The
   first is the use of unit tests to ensure that the software is doing
   as advertised. The second is the practice of committing (to master)
   running code. Maybe it would be better to break these out, and go
   for the novelty of 11, rather than the familiar 10, rules.
   
> Response: We refined the **Rule 5** and now it only provides information about
> unit tests and the idea of continuous integration.

8. In Rule 5 and in the context of unit tests (and also in the
   'automatic' generation of documentation), I think that many
   attempts at unit tests / documentation are superficial and
   misguided. At least from an anecdotal perspective, I'm sure we all
   are familiar with the information-less javadoc along the lines of
   'field foo is an integer that defines foo'. Certainly unit tests
   that validate inputs and even outputs are valuable. But somehow one
   would like to elevate unit tests of scientific software to the
   'next level', where the assertions of the mathematical closure
   implied by the unique analytic methods are evaluated, rather than
   merely the correctness of the inputs; one would like to do this in
   the spirit of unit, rather than integration, tests, and metrics
   like code coverage are imperfect at capturing this. Likewise I
   think attempts to 'automatically update the documentation on code
   modification' are almost counter-productive -- availability of this
   level of documentation is not really what users crave.
   
> Response: The idea of the manuscript is to show that the git/GitHub infrastructure
> can help the bioinformatics community to achieve general good programming
> practices. The problem with information-less documentation is
> certainly a valid one, but, to some extend independent of its
> automatic generation (although it might arguably invite developers
> to write useless documentation for the sake of it). We do address
> more fundamental applications of unit test, stressing out the
> testing of *logical errors*. And while one would want to perform
> scientificly-minded tests, these are often much more difficult to
> conceptualise and implement and, as experience has shown, thorough
> simple testing can uncover more serious problems. 

9. Rule 9 does not mention the obvious, effective, and esssential
   method for promoting one's project -- publishing in the
   peer-reviewed scientific literature!
   
> Response: The current version of the rule starts by stating: "The traditional
> way of promoting scientific software is by publishing them in the
> peer-reviewed scientific literature."

# Reviewer 3

I recommend the manuscript 'Ten Simple Rules for Taking Advantage of GitHub in
Bioinformatics' by Perez-Rivero et al should be accepted pending minor revisions
(see below).  The work on the paper isn't novel (lots of related articles and
guides for source code repos for life scientists) but this fits well within the
educational 'Ten Simple Rules' articles, and is a nice and pertinent
summarization of the key features of GitHub and specific use cases for scientists.

## Comments:

1. Small thing: I would suggest a minor title change to reflect that
   (even though this *is* going into PLOS CompBio) that the rules
   aren't just specific to bioinformatics. In fact, the term
   'bioinformatics' appears exactly exactly twice in the paper
   (leaving out the title and affiliations), both times in the
   'Introduction' text!  Beyond that, one could substitute any
   discipline for 'bioinformatics' as long as it required some need
   for version control. Maybe something like "Ten Simple Rules for
   Taking Advantage of GitHub for Scientists".  I'm horrible with
   titles, though, maybe I shouldn't come up with this :)
   
> Response: We agree with the reviewer. The new version of the mansucript has a different title: "# Ten
> Simple Rules for taking advantage of git and GitHub"

2. Pg. 1, Introduction, para1: "Here, we introduce the main features
   of GitHub, a popular web-based platform which offers a free and
   integrated environment for hosting the source code, documentation
   and web page for open source projects."

   Probably a better way to word ‘web page’, something like ‘public
   project-related web content’ since many projects are more complex.
  
> Response: We have followed the reviewer's advice and ammended the sentence:
> "Here, we introduce the main features of GitHub, a popular web-based
> platform which offers a free and integrated environment for hosting
> the source code, documentation and project-related web content for
> open source projects"

3. Pg. 2, Introduction, para 2: small revision suggestion 

   “These rules have been ordered to reflect a typical development
   process: learning git and GitHub basics, use of branches, labeling
   and tagging of code snapshots, tracking project bugs and
   enhancements using issues, etc”

> Response: We have updated that sentence following the reviewer's suggestion.

4. Pg. 2, Rule 1:

    a) Might be worth explaining what 'forking' means.
    
> Response: The revised version now includes a short explanation of the forking concept. 

    b) "Structuring your projects allows to manage permissions and restrict
    access at different levels: users, teams and organisations."  Maybe "Project
    managers can structure projects to manage…"

> Response: We agree with the reviewer and the current version includes the suggested change.

    c) Repositories: The bit on repositories should be described earlier, not at
    the end.  You are technically forking a *repository*, not just a project
    (which in my opinion could consist of many independent but related
    repositories, e.g. the Bio* projects, GMOD, etc).
    
> Response: We re-structured the rules and rule 1 is now more appropriate for
> new users.


5. Pg. 3, Rule 2:

    a) "The cornerstone of GitHub is the distributed version control system git.
    Every change, from fixing a typo to a complete redesign of the software, is
    controlled by versions, so-called revisions." (added a comma after
    'software')
    
> Response: We changed the sentence in the present version. 

6. Pg. 3, Rule 3:

    a) "Nevertheless, one can always pull the currently up-to date master branch
    into one branch, enabling one to react or adapt to the changes in the stable
    code branch." (use 'branch', not 'fork')
    
>  Response: We changed the sentence.

    b) "Once a pull request is opened for review and discussion, it usually
    results in additional insights and increased code quality" ('it' was
    ambiguous)

7. Pg. 5, Rule 8:

    a) "The main motivation behind this is to give scientists a better credit
    for their work".  True, but this is also key for grants and funding, where
    many funding agencies such as NIH now accept other 'products' of research as
    citable research (these being publicly accessible data and software).
    
> Response: We agree with the reviewer. The present version mentions also funding agencies.

    b) https://guides.github.com/activities/citable-code/
    Should be consistent w/ other URLs in text
    
> Response: This has been changed.

    c) ‘On one hand… on the other hand’ usually are used to describe two sides
    or opposing viewpoints. Not sure it’s used correctly here, since both
    examples are complementary, not in opposition to one another?
    
> Response: This has been ammended.

Chris Fields
