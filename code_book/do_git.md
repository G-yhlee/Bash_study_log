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
    echo '---status---\n'
    git status
    echo '---add all---'
    git add .
    echo "---commit msg: $1---"
    git commit -m $1
    echo "---push to main---"
    git push -u origin main
    echo "---LOG---"
    git log --all --decorate --oneline --graph  
} # 해당 파일이 실행 됩니다


```


