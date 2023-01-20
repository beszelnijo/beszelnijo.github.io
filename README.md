## Fejlesztői környezet
[Install Jekyll on Ubuntu in WSL](https://jekyllrb.com/docs/installation/ubuntu/)
```
bundle install
bundle exec jekyll serve --livereload
```
* A forrást wsl könyvtárba clonozzuk le pl.: ~/<project-name>
* VSCode-al kell megnyitni "open wsl"  a WSL könyvtárat
* A Git 2.35.2 óta nem a git nem kezeli a shared könyvtárakat https://github.blog/2022-04-12-git-security-vulnerability-announced/
Mivel a WSL és Windows user eltér ezért a trusted könyvtárak közé vagy a konkrét könyvtárat fel kell venni, vagy ha nem használja más a gépet, akkor a 
le is tudjuk tiltani.
https://stackoverflow.com/questions/71849415/i-cannot-add-the-parent-directory-to-safe-directory-in-git

https://git-scm.com/docs/git-config/2.35.2#Documentation/git-config.txt-safedirectory
git config --global --add safe.directory *
```
[safe]
  directory = *
```
* Windows-ban a WSL könyvtárat a ```explolrer.exe .``` tudjuk megnyitni  pl.: \\wsl.localhost\ubuntu\home\<usernam>\<projectname>
https://learn.microsoft.com/en-us/windows/wsl/filesystems

## Theme
https://themes.stackbit.com/demos/fresh/
* codesandbox.io-ról lett letölve a template  https://codesandbox.io/s/github/stackbithq/stackbit-theme-fresh/tree/master/
* régi github https://github.com/stackbithq/stackbit-theme-fresh az új https://github.com/stackbit
* egy fork lehet: https://github.com/Atinux/stackbit-theme-fresh
  