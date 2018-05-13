# Spring Bean

## Bean Scope

When you create a bean definition, you create a _recipe _for creating actual instances of the class defined by that bean definition. The idea that a bean definition is a recipe is important, because it means that, as with a class, you can create many object instances from a single recipe.

| Scope | Description |
| :--- | :--- |
| Singleton | Scopes a single bean definition to a single object instance per Spring IoC container. |
| Prototype | Scopes a single bean definition to any number of object instances. |
| Request | Scopes a single bean definition to the lifecycle of a single HTTP request; that is, each HTTP request has its own instance of a bean created off the back of a single bean definition. Only valid in the context of a web-aware Spring ApplicationContext. |
| Session | Scopes a single bean definition to the lifecycle of an HTTP Session. Only valid in the context of a web-aware Spring ApplicationContext. |
| Global Session | Scopes a single bean definition to the lifecycle of a global HTTP Session. Typically only valid when used in a portlet context. Only valid in the context of a web-aware Spring ApplicationContext. |



## Bean Life cycle



![](/assets/bean life cycle.png)

