
##  我们如何用状态机处理完全未知的 pattern
### 源码
https://codesandbox.io/s/kmp-string-matcher-r2voq   
### 测试结果
[test-result](./images/test-result.png)

### 思路
1. 先根据 pattren 创建 pattren 每个字符对应的部分匹配值
2. 创建保存状态机的数组
3. 根据 pattren 的每个字符创建状态函数并保存到数组
4. 返回第一个状态函数

---

## 完成 toy-browser 的 dom 树和 css 计算部分

### 完成的可选作业
- 实现了复合选择器
- 实现 class 选择器   
以上可选作业均已完成  

### 源码
https://github.com/jinglen/toy-browser/tree/master/src/toyBrowser

### 预览
https://jinglen.github.io/toy-browser


