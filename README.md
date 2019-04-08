# Big-Talk-Design-Model
菜鸟成长史 设计模式学习

> 菜鸟手记 代码无错就是优？ 简单工厂模式
```
class Factory{
    public static Operation createFactory(String use){
        Operation oper = null;
        switch (use) {
            case "+":
                oper = new OperationAdd();
                break;
            case "-":
                oper = new OperationSub();
                break;
            case "*":
                oper = new OperationSub();
                break;
            default:
                break;
        }
        return oper;
    }
}
```