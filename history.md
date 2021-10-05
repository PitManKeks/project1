   50  sudo apt install git-all
   51  git --version
   52  git config --global user.name "Шульдяков"
   53  git config --global user.email "pitmankeks@gmail.com"
   54  ssh-keygen -t rsa -b 4096 -C "pitmankeks@gmail.com"
   55  cd ~/.ssh
   56  ls
   57  eval "$(ssh-agent -s)"
   58  ssh-add ~/.ssh/id_rsa
   59  cat ~/.ssh/id_rsa.pub
   60  mkdir project1
   61  cd project1
   62  touch Readme.md
   63  nano Readme.md
   64  git init
   65  git add .
   66  git commit -m "First commit"
   67  git remote add origin git@github.com:PitManKeks/project1.git
   68  curl -u 'PitManKeks:****************************************' https://api.github.com/user/repos -d '{"name":"project1"}'
   69  git push -u origin master
   70  git checkout -b firstbranch
   71  history
