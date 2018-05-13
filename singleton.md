```java
// ENUM
public enum Singleton{
    INSTANCE;
    public void whateverMethod(){}
}
```



```java
//double check
public class Singleton{
    private volatile static Singleton singleton;
    private Sinlgeton(){}
    public static Singleton getSingleton(){
        if(singleton == null){
            synchronized (Singleton.class){
                if(singleton == bull){
                    singleton = new Singleton();
                }
            }
        }
        return singleton;
    }
}
```

```java
//static class
public class Singleton{
    private static class SingletonHolder {
        private static final Singleton INSTANCE = new Singleton();  
    }
    private Singleton (){}
    public static final Singleton getInstance() {  
        return SingletonHolder.INSTANCE;  
    }  
}
```



