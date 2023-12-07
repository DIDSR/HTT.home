# HTT.home
Live site: [https://didsr.github.io/HTT.home/](https://didsr.github.io/HTT.home/)

## How to connect to a virtual machine over SSH
[VS Code: Remote Development over SSH](https://code.visualstudio.com/docs/remote/ssh-tutorial) 
1.	Install ‘Remote – SSH’ extension in VSCode: vscode:extension/ms-vscode-remote.remote-ssh
2.	Click the remote server button in the bottom left corner of VSCode (Icon looks like an unleveled > <) 
3.	Choose “Connect to Host..”  
4.	Enter SSH host: 172.31.151.221 (port 22)
5.	Put in username and password of openHPC
6.	If it worked, the bottom left corner banner will now show the Remote host icon and “SSH: 172.31.151.221”
7.	Follow all steps prompted by VScode

## Adding remote repository connection (ie. cloning)
[GitHub Docs: Managing Remote Repositories](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories)  
[Free Code Camp: Fetching Remote Branches](https://www.freecodecamp.org/news/git-pull-remote-branch-how-to-fetch-remote-branches-in-git/#:~:text=You%20can%20do%20this%20with,or%20inspect%20at%20any%20time.)  
[Git: First Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)  

1.	In the Terminal, use `git remote add origin git@github.com:DIDSR/HTT.home.git`
2.	Verify new remote with `git remote -v`
3.	Add github account information to git config 
a.	`git config --global user.name “[[username]]”`
b.	`git config --global user.email [[userEmail]]`
4.	Check git branches `git branch -r`
5.	Specify default branch `git config --global init.defaultBranch [[branchName]]`
6.	Check git config file `git config --list` 
7.	To download repo changes use `git pull origin` for all branches changes
8.	Then `git checkout` to merge the changes
9.	If you want to download and merge in one: use `git pull --all`

## Adding gems
1.	Configure bundler for project in Terminal: `bundle config set path vendor/bundle`  
    Mine: bundle config set path /home/emma.gardecki/.local/share/gem/ruby/3.1.0/bin  
    Should create a file /.bundle/config with the BUNDLE_PATH  
2.	Use `gem install --user-install [[gem_name]]`  
    List of gems:    
        i.	bundle  
        ii.	bundler  
        iii.	commonmarker  
        iv.	gemoji  
        v.	github-pages  
        vi.	jekyll  
        vii.	kramdown  
        viii.	listen  
        ix.	nokogiri  
        x.	racc  
        xi.	rake  
        xii.	rougify  
        xiii.	sass  
        xiv.	sass-convert  
        xv.	scss  
3.	Update gems `gem update`  
4.	Update bundle `bundle update` -> this could make changes to Gemfile and Gemfile.Lock  

## Locally deploy site
1.	If changes to any gems or config, `bundle update`  
2.	To locally deploy, `bundle exec jekyll serve`  

## Regular git terminal actions
[GitHub issue: Detatched Head State Fix](https://github.com/desktop/desktop/issues/16244)  
* The easier way to commit is using the Source Control icon on the right toolbar in VSCode, write message, stage commits and push all right there

1.	If you want to download and merge in one: use `git pull --all`  
2.	To commit changes `git commit -m ` for short message changes  
    To make long message commit `git commit` which will open Vim interface for commit message  
3.	To push changes `git push origin [[branchname]]`  
4.	To check connection `git fsck`  
5.	To switch between branches `git switch [[branchname]]`  
6.	To remove remote connection, `git remote rm [[branchname]]`
7.	Add file to commit, `git add [file path]`
8.	Check what commits are staged, `git status`
9.	If you want to download and merge in one: use `git pull --all`
10.	Make new branch, `git checkout -b [branchName]`
11.	Make commit, `git commit -m "[message]"`
12.	Connect newBranch to server, `git push origin -u [branchName]` (only need to do this with first commit of a new branch)


## Notes
* Information at the bottom of each page is found in this file
  * _includes/footer.html
