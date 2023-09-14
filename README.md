# omz_git_cheatsheet_howto

HOWTO use git aliases with oh_my_zsh

## git add
[Алиас](howto.md#ga): `ga` **Команда:** `git add`  
[Алиас](howto.md#gaa): `gaa` **Команда:** `git add --all`  
[Алиас](howto.md#gapa): `gapa` **Команда:** `git add --patch`  
[Алиас](howto.md#gau): `gau` **Команда:** `git add --update`  
[Алиас](howto.md#gav): `gav` **Команда:** `git add --verbose`  

## git apply
[Алиас](howto.md#gap): `gap` **Команда:** `git apply`  
[Алиас](howto.md#gapt): `gapt` **Команда:** `git apply --3way`  

## git branch
[Алиас](howto.md#gb): `gb` **Команда:** `git branch`  
[Алиас](howto.md#gba): `gba` **Команда:** `git branch -a`  
[Алиас](howto.md#gbd): `gbd` **Команда:** `git branch -d`  
[Алиас](howto.md#gbda): `gbda` **Команда:** `git branch --no-color --merged | grep -vE "^([+]|\s($(git_main_branch)|$(git_develop_branch))\s*$)" | xargs git branch -d 2>/dev/null`  
[Алиас](howto.md#gbD): `gbD` **Команда:** `git branch -D`  
[Алиас](howto.md#gbnm): `gbnm` **Команда:** `git branch --no-merged`  
[Алиас](howto.md#gbr): `gbr` **Команда:** `git branch --remote`  
[Алиас](howto.md#ggsup): `ggsup` **Команда:** `git branch --set-upstream-to=origin/$(git_current_branch)`  

## git blame
[Алиас](howto.md#gbl): `gbl` **Команда:** `git blame -b -w`  

## git bisect
[Алиас](howto.md#gbs): `gbs` **Команда:** `git bisect`  
[Алиас](howto.md#gbsb): `gbsb` **Команда:** `git bisect bad`  
[Алиас](howto.md#gbsg): `gbsg` **Команда:** `git bisect good`  
[Алиас](howto.md#gbsr): `gbsr` **Команда:** `git bisect reset`  
[Алиас](howto.md#gbss): `gbss` **Команда:** `git bisect start`  

## git commit
[Алиас](howto.md#gc): `gc` **Команда:** `git commit -v`  
[Алиас](howto.md#gc): `gc!` **Команда:** `git commit -v --amend`  
[Алиас](howto.md#gcn): `gcn!` **Команда:** `git commit -v --no-edit --amend`  
[Алиас](howto.md#gca): `gca` **Команда:** `git commit -v -a`  
[Алиас](howto.md#gca): `gca!` **Команда:** `git commit -v -a --amend`  
[Алиас](howto.md#gcan): `gcan!` **Команда:** `git commit -v -a --no-edit --amend`  
[Алиас](howto.md#gcans): `gcans!` **Команда:** `git commit -v -a -s --no-edit --amend`  
[Алиас](howto.md#gcam): `gcam` **Команда:** `git commit -a -m`  
[Алиас](howto.md#gcas): `gcas` **Команда:** `git commit -a -s`  
[Алиас](howto.md#gcasm): `gcasm` **Команда:** `git commit -a -s -m`  
[Алиас](howto.md#gcsm): `gcsm` **Команда:** `git commit -s -m`  
[Алиас](howto.md#gcmsg): `gcmsg` **Команда:** `git commit -m`  
[Алиас](howto.md#gcs): `gcs` **Команда:** `git commit -S`  

## git checkout
[Алиас](howto.md#gcb): `gcb` **Команда:** `git checkout -b`  
[Алиас](howto.md#gcm): `gcm` **Команда:** `git checkout $(git_main_branch)`  
[Алиас](howto.md#gcd): `gcd` **Команда:** `git checkout $(git_develop_branch)`  
[Алиас](howto.md#gco): `gco` **Команда:** `git checkout`  
[Алиас](howto.md#gcor): `gcor` **Команда:** `git checkout --recurse-submodules`  

## git config
[Алиас](howto.md#gcf): `gcf` **Команда:** `git config --list`  

## git clone
[Алиас](howto.md#gcl): `gcl` **Команда:** `git clone --recurse-submodules`  
[Алиас](howto.md#gccd): `gccd` **Команда:** `git clone --recurse-submodules "$@" && cd "$(basename $_ .git)"`  

## git cherry-pick
[Алиас](howto.md#gcp): `gcp` **Команда:** `git cherry-pick`  
[Алиас](howto.md#gcpa): `gcpa` **Команда:** `git cherry-pick --abort`  
[Алиас](howto.md#gcpc): `gcpc` **Команда:** `git cherry-pick --continue`  

## git diff
[Алиас](howto.md#gd): `gd` **Команда:** `git diff`  
[Алиас](howto.md#gdca): `gdca` **Команда:** `git diff --cached`  
[Алиас](howto.md#gdcw): `gdcw` **Команда:** `git diff --cached --word-diff`  
[Алиас](howto.md#gds): `gds` **Команда:** `git diff --staged`  
[Алиас](howto.md#gdt): `gdt` **Команда:** `git diff-tree --no-commit-id --name-only -r`  
[Алиас](howto.md#gdnolock): `gdnolock` **Команда:** `git diff $@ ":(exclude)package-lock.json" ":(exclude)*.lock"`  
[Алиас](howto.md#gdup): `gdup` **Команда:** `git diff @{upstream}`  
[Алиас](howto.md#gdv): `gdv` **Команда:** `git diff -w $@ | view -`  
[Алиас](howto.md#gdw): `gdw` **Команда:** `git diff --word-diff`  

## git push
[Алиас](howto.md#ggf): `ggf` **Команда:** `git push --force origin $(current_branch)`  
[Алиас](howto.md#ggfl): `ggfl` **Команда:** `git push --force-with-lease origin $(current_branch)`  
[Алиас](howto.md#ggp): `ggp` **Команда:** `git push origin $(current_branch)`  
[Алиас](howto.md#ggpush): `ggpush` **Команда:** `git push origin "$(git_current_branch)"`  
[Алиас](howto.md#gpsup): `gpsup` **Команда:** `git push --set-upstream origin $(git_current_branch)`  

[Алиас](howto.md#gp): `gp` **Команда:** `git push`  
[Алиас](howto.md#gpd): `gpd` **Команда:** `git push --dry-run`  
[Алиас](howto.md#gpf): `gpf` **Команда:** `git push --force-with-lease`  
[Алиас](howto.md#gpf): `gpf!` **Команда:** `git push --force`  
[Алиас](howto.md#gpoat): `gpoat` **Команда:** `git push origin --all && git push origin --tags`  
[Алиас](howto.md#gpu): `gpu` **Команда:** `git push upstream`  
[Алиас](howto.md#gpv): `gpv` **Команда:** `git push -v`  

## git log
[Алиас](howto.md#gke): `gke` **Команда:** `gitk --all $(git log -g --pretty=%h) &!`  
[Алиас](howto.md#glg): `glg` **Команда:** `git log --stat`  
[Алиас](howto.md#glgp): `glgp` **Команда:** `git log --stat -p`  
[Алиас](howto.md#glgg): `glgg` **Команда:** `git log --graph`  
[Алиас](howto.md#glgga): `glgga` **Команда:** `git log --graph --decorate --all`  
[Алиас](howto.md#glgm): `glgm` **Команда:** `git log --graph --max-count=10`  
[Алиас](howto.md#glo): `glo` **Команда:** `git log --oneline --decorate`  
[Алиас](howto.md#glol): `glol` **Команда:** `git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%ar) %C(bold blue)<%an>%Creset'`  
[Алиас](howto.md#glols): `glols` **Команда:** `git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%ar) %C(bold blue)<%an>%Creset' --stat`  
[Алиас](howto.md#glod): `glod` **Команда:** `git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%ad) %C(bold blue)<%an>%Creset'`  
[Алиас](howto.md#glods): `glods` **Команда:** `git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%ad) %C(bold blue)<%an>%Creset' --date=short`  
[Алиас](howto.md#glola): `glola` **Команда:** `git log --graph --pretty='%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%ar) %C(bold blue)<%an>%Creset' --all`  
[Алиас](howto.md#glog): `glog` **Команда:** `git log --oneline --decorate --graph`  
[Алиас](howto.md#gloga): `gloga` **Команда:** `git log --oneline --decorate --graph --all`  
[Алиас](howto.md#glp): `glp` **Команда:** `git log --pretty=<format>`  


## git rebase
[Алиас](howto.md#grb): `grb` **Команда:** `git rebase`  
[Алиас](howto.md#grba): `grba` **Команда:** `git rebase --abort`  
[Алиас](howto.md#grbc): `grbc` **Команда:** `git rebase --continue`  
[Алиас](howto.md#grbd): `grbd` **Команда:** `git rebase $(git_develop_branch)`  
[Алиас](howto.md#grbi): `grbi` **Команда:** `git rebase -i`  
[Алиас](howto.md#grbm): `grbm` **Команда:** `git rebase $(git_main_branch)`  
[Алиас](howto.md#grbom): `grbom` **Команда:** `git rebase origin/$(git_main_branch)`  
[Алиас](howto.md#grbo): `grbo` **Команда:** `git rebase --onto`  
[Алиас](howto.md#grbs): `grbs` **Команда:** `git rebase --skip`  

## git stash
[Алиас](howto.md#gsta): `gsta` **Команда:** `git stash push`  
[Алиас](howto.md#gstaa): `gstaa` **Команда:** `git stash save`  
[Алиас](howto.md#gstc): `gstc` **Команда:** `git stash apply`  
[Алиас](howto.md#gstd): `gstd` **Команда:** `git stash clear`  
[Алиас](howto.md#gstl): `gstl` **Команда:** `git stash drop`  
[Алиас](howto.md#gstp): `gstp` **Команда:** `git stash list`  
[Алиас](howto.md#gsts): `gsts` **Команда:** `git stash pop`  
[Алиас](howto.md#gstu): `gstu` **Команда:** `git stash show --text`  
[Алиас](howto.md#gstall): `gstall` **Команда:** `git stash --include-untracked`  
[Алиас](howto.md#gsu): `gsu` **Команда:** `git stash --all`  

## git remote
[Алиас](howto.md#gr): `gr` **Команда:** `git remote`  
[Алиас](howto.md#gra): `gra` **Команда:** `git remote add`  
[Алиас](howto.md#grmv): `grmv` **Команда:** `git remote rename`  
[Алиас](howto.md#grrm): `grrm` **Команда:** `git remote remove`  
[Алиас](howto.md#grset): `grset` **Команда:** `git remote set-url`  
[Алиас](howto.md#grup): `grup` **Команда:** `git remote update`  
[Алиас](howto.md#grv): `grv` **Команда:** `git remote -v`  

## git pull
[Алиас](howto.md#ggl): `ggl` **Команда:** `git pull origin $(current_branch)`  
[Алиас](howto.md#ggpull): `ggpull` **Команда:** `git pull origin "$(git_current_branch)"`  
[Алиас](howto.md#ggu): `ggu` **Команда:** `git pull --rebase origin $(current_branch)`  
[Алиас](howto.md#gl): `gl` **Команда:** `git pull`  
[Алиас](howto.md#gpr): `gpr` **Команда:** `git pull --rebase`  
[Алиас](howto.md#gupv): `gupv` **Команда:** `git pull --rebase`  
[Алиас](howto.md#gupa): `gupa` **Команда:** `git pull --rebase -v`  
[Алиас](howto.md#gupav): `gupav` **Команда:** `git pull --rebase --autostash`  
[Алиас](howto.md#gupom): `gupom` **Команда:** `git pull --rebase --autostash -v`  
[Алиас](howto.md#gupomi): `gupomi` **Команда:** `git pull --rebase origin $(git_main_branch)`  
[Алиас](howto.md#glum): `glum` **Команда:** `git pull --rebase=interactive origin $(git_main_branch)`  
[Алиас](howto.md#gluc): `gluc` **Команда:** `git pull upstream $(git_main_branch)`  
[Алиас](howto.md#gwch): `gwch` **Команда:** `git pull upstream $(git_current_branch)`  

## git switch
[Алиас](howto.md#gswc): `gswc` **Команда:** `git switch`  
[Алиас](howto.md#gswm): `gswm` **Команда:** `git switch -c`  
[Алиас](howto.md#gswd): `gswd` **Команда:** `git switch $(git_main_branch)`  
[Алиас](howto.md#gts): `gts` **Команда:** `git switch $(git_develop_branch)`  

## git fetch
[Алиас](howto.md#gf): `gf` **Команда:** `git fetch`  
[Алиас](howto.md#gfa): `gfa` **Команда:** `git fetch --all --prune`  
[Алиас](howto.md#gfo): `gfo` **Команда:** `git fetch origin`  

## git mergetool
[Алиас](howto.md#gmtl): `gmtl` **Команда:** `git mergetool --no-prompt`  
[Алиас](howto.md#gmtlvim): `gmtlvim` **Команда:** `git mergetool --no-prompt --tool=vimdiff`  

## git merge
[Алиас](howto.md#gm): `gm` **Команда:** `git merge`  
[Алиас](howto.md#gmom): `gmom` **Команда:** `git merge origin/$(git_main_branch)`  
[Алиас](howto.md#gmum): `gmum` **Команда:** `git merge upstream/$(git_main_branch)`  
[Алиас](howto.md#gma): `gma` **Команда:** `git merge --abort`  

## git status
[Алиас](howto.md#gsb): `gsb` **Команда:** `git status -sb`  
[Алиас](howto.md#gss): `gss` **Команда:** `git status -s`  
[Алиас](howto.md#gst): `gst` **Команда:** `git status`  

## git restore
[Алиас](howto.md#grs): `grs` **Команда:** `git restore`  
[Алиас](howto.md#grss): `grss` **Команда:** `git restore --source`  
[Алиас](howto.md#grst): `grst` **Команда:** `git restore --staged`  


## git reset
[Алиас](howto.md#gup): `gup` **Команда:** `git log -n 1 | grep -q -c "--wip--" && git reset HEAD~1`  
[Алиас](howto.md#gpristine): `gpristine` **Команда:** `git reset --hard && git clean -dffx`  
[Алиас](howto.md#grh): `grh` **Команда:** `git reset`  
[Алиас](howto.md#grhh): `grhh` **Команда:** `git reset --hard`  
[Алиас](howto.md#groh): `groh` **Команда:** `git reset origin/$(git_current_branch) --hard`  
[Алиас](howto.md#gru): `gru` **Команда:** `git reset --`  

## git svn
[Алиас](howto.md#gsd): `gsd` **Команда:** `git svn dcommit`  
[Алиас](howto.md#gsr): `gsr` **Команда:** `git svn rebase`  

## git am
[Алиас](howto.md#gamcgamc): `gamc` **Команда:** `git am`  
[Алиас](howto.md#gamsgams): `gams` **Команда:** `git am --continue`  
[Алиас](howto.md#gamagama): `gama` **Команда:** `git am --skip`  
[Алиас](howto.md#gamscpgamscp): `gamscp` **Команда:** `git am --abort`  

## git submodule
[Алиас](howto.md#gsi): `gsi` **Команда:** `git submodule init`  
[Алиас](howto.md#gsw): `gsw` **Команда:** `git submodule update`  

## git rm
[Алиас](howto.md#gam): `gam` **Команда:** `git add -A; git rm $(git ls-files --deleted) 2> /dev/null; git commit --no-verify --no-gpg-sign -m " --wip-- [skip ci]"`  
[Алиас](howto.md#grm): `grm` **Команда:** `git rm`  
[Алиас](howto.md#grmc): `grmc` **Команда:** `git rm --cached`  

## git gui
[Алиас](howto.md#gg): `gg` **Команда:** `git gui citool`  
[Алиас](howto.md#gga): `gga` **Команда:** `git gui citool --amend`  

## git tag
[Алиас](howto.md#gtv): `gtv` **Команда:** `git tag -s`  
[Алиас](howto.md#gtl): `gtl` **Команда:** `git tag | sort -V`  
[Алиас](howto.md#gunignore): `gunignore` **Команда:** `gtl(){ git tag --sort=-v:refname -n -l ${1}* }; noglob gtl`  

## git show
[Алиас](howto.md#gsh): `gsh` **Команда:** `git show`  
[Алиас](howto.md#gsps): `gsps` **Команда:** `git show --pretty=short --show-signature`  

все остальное
[Алиас](howto.md#g): `g` **Команда:** `git`  
[Алиас](howto.md#gclean): `gclean` **Команда:** `git clean -id`  
[Алиас](howto.md#gcount): `gcount` **Команда:** `git shortlog -sn`  
[Алиас](howto.md#gdct): `gdct` **Команда:** `git describe --tags $(git rev-list --tags --max-count=1)`  
[Алиас](howto.md#gfg): `gfg` **Команда:** `git ls-files | grep`  
[Алиас](howto.md#ggpnp): `ggpnp` **Команда:** `ggl && ggp`  
[Алиас](howto.md#ggpur): `ggpur` **Команда:** `ggu`  
[Алиас](howto.md#ghh): `ghh` **Команда:** `git help`  
[Алиас](howto.md#gignore): `gignore` **Команда:** `git update-index --assume-unchanged`  
[Алиас](howto.md#gignored): `gignored` **Команда:** `git ls-files -v | grep "^[[:lower:]]"`  
[Алиас](howto.md#gk): `gk` **Команда:** `gitk --all --branches &!`  
[Алиас](howto.md#grev): `grev` **Команда:** `git revert`  
[Алиас](howto.md#grt): `grt` **Команда:** `cd "$(git rev-parse --show-toplevel || echo .)"`  
[Алиас](howto.md#gunwip): `gunwip` **Команда:** `git update-index --no-assume-unchanged`  
[Алиас](howto.md#gwip): `gwip` **Команда:** `git whatchanged -p --abbrev-commit --pretty=medium`  





[Aliases source](https://kapeli.com/cheat_sheets/Oh-My-Zsh_Git.docset/Contents/Resources/Documents/index)
