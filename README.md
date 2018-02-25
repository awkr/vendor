# vendor

## 新加某个库

1. git remote add protobuf https://github.com/golang/protobuf.git
2. gco master; gco -b feature/github.com/golang/protobuf
3. git subtree add --prefix=github.com/golang/protobuf/ protobuf master --squash
4. gco master; git merge feature/github.com/golang/protobuf

或者较简洁的：
git subtree add --prefix=google.golang.org/genproto/ https://github.com/google/go-genproto.git master --squash

## 更新某个库

git subtree pull --prefix=github.com/golang/protobuf/ protobuf master
