> fat-thursday-7
# Jak być GIT z VSCode?

## Czego potrzebujemy do optymalnej pracy z GIT'em w VSCode?
### [**GITLense**](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
![GITLens Logo](https://eamodio.gallerycdn.vsassets.io/extensions/eamodio/gitlens/11.7.0/1637268068613/Microsoft.VisualStudio.Services.Icons.Default )
>GitLens supercharges the Git capabilities built into Visual Studio Code. It helps you to visualize code authorship at a glance via Git blame annotations and code lens, seamlessly navigate and explore Git repositories, gain valuable insights via powerful comparison commands, and so much more.

### [**GIT Graph**](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
![GITLens Logo](https://mhutchie.gallerycdn.vsassets.io/extensions/mhutchie/git-graph/1.30.0/1617594001998/Microsoft.VisualStudio.Services.Icons.Default )

>View a Git Graph of your repository, and easily perform Git actions from the graph. Configurable to look the way you want!

### [**GIT History**](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) 
![GITLens Logo](https://donjayamanne.gallerycdn.vsassets.io/extensions/donjayamanne/githistory/0.6.19/1635531678980/Microsoft.VisualStudio.Services.Icons.Default)

>Git History, Search and More (including git log)

[*Instrukcja jak zainstalować wtyczki w VSCode.*](https://code.visualstudio.com/docs/editor/extension-marketplace)

---

## Praca z podstawowymi poleceniami- czyli to czego używamy najczęściej

### `git clone`

Można wybrać tryb klonowania prosto z podanego URL'a bądz jeśli wybierzemy opcję GitHub i sparujemy nasz VSCode z kontem na Githubie, będziemy mogli klonować repozytoria które są na naszym koncie. 
Warto wspomnieć w tym miejcu o wtyczce [GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) dzięki której możemy przeglądać i zarządzać GitHubowymi pull requestami bezpośrednio z poziomu VSCode. Istnieje także jej odpowiednik dla BitBucketa [Jira and Bitbucket](https://marketplace.visualstudio.com/items?itemName=Atlassian.atlascode)

### `git add`

Zmiany jakie chcemy zacommitować wybieramy w panelu *Source Control*. Możemy dodawać do commita całe pliki lub wybrać tylko te linnie kodu które nas interesują -> w tym celu wyświetlamy *working tree* w exploratorze, zaznaczamy interesującą nasz część i z menu kontekstowego wybieramy `Stage Selected Ranges` (lub używamy skrótu klawiaturowego *CMD + K ALT + CMD + S*). Możemu tutaj także odznaczyć kod który nas nie interesuje, albo cofnąć nasze zmiany. 

Istnieje jeszcze możliwość *stagowania* zmian bezpośrednio w edytowanym pliku -> więcej o tym będzie przy **rewizji**. 

Ekwiwalent tych opcji to polecenie 
```properties
git add --patch
```

### `git commit`
Polecenie `git commit` możemy wywołać bezpośrednio z *command palette* (mamy tam kilka opcji), oraz takzę w panelu `Source control`. 
