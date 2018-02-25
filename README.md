# vendor

## 新加某个库

1. git remote add protobuf https://github.com/golang/protobuf.git
2. gco master; gco -b feature/github.com/golang/protobuf
3. git subtree add --prefix=github.com/golang/protobuf/ protobuf master --squash
4. gco master; git merge feature/github.com/golang/protobuf

## 更新某个库

git subtree pull --prefix=github.com/golang/protobuf/ protobuf master
