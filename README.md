# go-a13

每个文件夹都是一个独立的mod, 打标签规则 m1/v1.0.0, 引用规则
```
github.com/relax-space/go-a13/m1@v1.0.0
```

## go work
当m1和m2都mod init之后, 就可以执行下面的代码, 保证gopls正常
```
go work init ./m1
go work use ./m2
```