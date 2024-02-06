# Basic git commands  
### Basic commands  
`git init` - make the folder a repository  
`rm -rf .git` - remove repo characteristic folder  
`git status` - show git status


`git add` - prepearing files for saving


`git commit` - to make a commit


`git push` - submitting to a public repository  


### SSH  
`ssh-keygen -t ed25519 -C "my git e-mail"` - prepearing files for saving  
`clip < ...id_rsa.pub` - copy public key to buffer  


### Connection between local and remote repos  
```
git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git
```

### GIT Statuses
- **`untracked`** (англ. «неотслеживаемый»)  
Мы говорили, что новые файлы в Git-репозитории помечаются как `untracked`, то есть неотслеживаемые. Git «видит», что такой файл существует, но не следит за изменениями в нём. У `untracked`файла нет предыдущих версий, зафиксированных в коммитах или через команду `git add`.
- **`staged`** (англ. «подготовленный»)  
После выполнения команды `git add` файл попадает в **staging area** (от англ. *stage* — «сцена», «этап [процесса]» и *area* — «область»), то есть в список файлов, которые войдут в коммит. В этот момент файл находится в состоянии `staged`.
- **`tracked`** (англ. «отслеживаемый»)  
Состояние `tracked` — это противоположность `untracked`. Оно довольно широкое по смыслу: в него попадают файлы, которые уже были зафиксированы с помощью `git commit`, а также файлы, которые были добавлены в staging area командой `git add`. То есть все файлы, в которых Git так или иначе отслеживает изменения.
- **`modified`** (англ. «изменённый»)  
Состояние `modified` означает, что Git сравнил содержимое файла с последней сохранённой версией и нашёл отличия. Например, файл был закоммичен и после этого изменён.  



