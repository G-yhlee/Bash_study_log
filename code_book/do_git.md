```bash
function g-ad {
    git add .
} # 해당 파일이 실행 됩니다

function g-cm {
    git commit -m $1
} # 해당 파일이 실행 됩니다

function g-st {
    git status
} # 해당 파일이 실행 됩니다

function g-start {
    git init
    git add .
    git commit -m 'i'
} # 해당 파일이 실행 됩니다

function g-log {
    echo 'g-log 실행'
    git log --all --decorate --oneline --graph
} # 해당 파일이 실행 됩니다
function g-push {
    echo '---status---'
    echo ' '
    git status
    echo ' '
    echo '---add all---'
    echo ' '
    git add .
    echo ' '
    echo "---commit msg: $1---"
    echo ' '
    git commit -m $1
    echo ' '
    echo "---push to main---"
    echo ' '
    git push -u origin main
    echo ' '
    echo "---LOG---"
    echo ' '
    git log --all --decorate --oneline --graph  
} # 해당 파일이 실행 됩니다


```


