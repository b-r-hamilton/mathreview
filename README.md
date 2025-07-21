# mathreview
Before the beginning of this Math Review session, please 
- [set up a GitHub account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)
- [download git](https://git-scm.com/downloads) 
- [set up an SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) (if you are on Windows, run these instructions through Git Bash)
- Slack message your GitHub username to Brynn and she will add you as a collaborator to the repository
  
Brynn will be in Clark 271 30 minutes before the beginning of class if you need help with any of these steps

# Demonstration: [how to set up a GitHub repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) 
_follow along, or just watch!_ 

git was invented in 2005 by Linus Torvalds to manage the development of Linux. In software years, that's centuries ago. Because of that, many different tools and ways to use git have been developed over the years. There are many ways to do steps I'm demonstrating here, but the important thing is to have a mental picture of what's happening. We'll use the GitHub website to create a repository, and then command line to modify our code and interface with the remote. 
1. Go to your GitHub 
2. Hit the (+) button
3. Create a new repository
4. Clone the repository locally
   ```
   git clone git@github.com:b-r-hamilton/mathreview.git
   ```
   _What does this command do?_

   `git`: tells the computer we want to use git

   `clone`: we want to create a perfect copy of something remote, locally

   `git@github.com:b-r-hamilton/mathreview.git`: this is our **remote**, the version of our code that is hosted somewhere else (in this case, on the GitHub server)
5. Make a local branch
   ```
   git branch [branch name] 
   ```
   _What does this command do?_ 
   
   `branch`: creates a branch off of main 

6. [Check out](https://git-scm.com/docs/git-checkout) the local branch 
   ```
   git checkout [branch name] 
   ```
7. Check [status](https://git-scm.com/docs/git-status)
   ```
   git status
   ```
   ```
    On branch main
   
    Your branch is up to date with 'origin/main'.
    
    Changes to be committed:
      (use "git restore --staged <file>..." to unstage)
    	modified:   README.md
   ```
8. [Stage](https://git-scm.com/docs/git-stage) or [add](https://git-scm.com/docs/git-add) changes
   ```
   git add [modified files] 
   ```
9. [Commit](https://git-scm.com/docs/git-commit)
   ```
   git commit -m `[message]`
   ```   
10. [Push](https://git-scm.com/docs/git-push)
    ```
    git push --set-upstream origin [branch name] 
    ```
    _What does this command do?_
   
   `push`: pushes the commits on branch [branch name] to the origin/main branch of the repository 
   
   `--set-upstream`: a flag to tell git that the [branch name] currently doesn't exist on the remote, so we need to initiate it there 
   
   `origin`: this means the remote repository 

   ```
   Enumerating objects: 5, done.
   Counting objects: 100% (5/5), done.
   Delta compression using up to 8 threads
   Compressing objects: 100% (2/2), done.
   Writing objects: 100% (3/3), 298 bytes | 298.00 KiB/s, done.
   Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
   remote: Resolving deltas: 100% (1/1), completed with 1 local object.
   remote: 
   remote: Create a pull request for 'frogs' on GitHub by visiting:
   remote:      https://github.com/b-r-hamilton/mathreview/pull/new/frogs
   remote: 
   To github.com:b-r-hamilton/mathreview.git
    * [new branch]      frogs -> frogs
   Branch 'frogs' set up to track remote branch 'frogs' from 'origin'.
   ```
11. Open a pull request 

Naviage to the repository on GitHub, you should see a notification that says your branch has changes, navigate to your branch, and then click "open a pull request" 
# Further Resources
- WHOI High Performance Compute Cluster (Poseidon)
   - [WHOI IS HPC Guide](https://whoi-it.whoi.edu/resources/) 
   - [Pad Poemnamthip's (JP Student) 2024 Math Review introduction to Poseidon](https://github.com/phadtaya/MITWHOI-ApplCoding/blob/main/IntroPoseidon.md)
   - [Colette Kelly's (WHOI Postdoc) Poseidon tutorial](https://boom.science/2023/10/03/poseidon-basics.html) 
- git
   - git-scm [git tutorial](https://git-scm.com/docs/gittutorial)
   - [Joe Futrelle's (WHOI IS specialist) presentation](https://github.com/WHOIGit/whoi-git-workshop)
   - [Learn Git Branching](https://learngitbranching.js.org/?locale=en_US)
- Python for geosciences
   - [University of Helsinki Geo-Python Tutorials](https://geo-python-site.readthedocs.io/en/latest/)
   - [Ryan Abernathey's "An Introduction to Earth and Environmental Data Science"](https://earth-env-data-science.github.io/intro.html)
- File System Organization
  - [PARA Method]{https://fortelabs.com/blog/para/}
  - [JohnnyDecimal]{https://johnnydecimal.com/}
