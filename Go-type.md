# type关键词总结

### type 用法：

* 定义结构体
* 定义接口 
* 类型别名 
* 类型定义
* 类型开关

### Type常见Demo

###### 定义结构体
```
type Demo struct {}

```

###### 定义接口
```
type Demoer interface {}

```

###### 类型别名
```
type Demo string

```

###### 类型定义
```
type handle func(str string) 

```

###### 类型开关
```
func Demo(params ...interface{})  {
   for i, x := range params {
      switch x.(type) {
      case bool:
         fmt.Printf("type #%d is bool",i)
      default:
         fmt.Printf("type is unknow")
      }
   }
}

```

