

## **IModelMapper.Load&#60;TModel>(ISqlQueryBuilder queryBuilder, params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

根据一个SqlQueryBuilder实例中定义的SQL检索规则检索数据。

Retrieves data according to the SQL query defined in the SqlQueryBuilder instance.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public ILoadable<TModel> Load<TModel>(ISqlQueryBuilder queryBuilder, params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standards.

**Parameters**

`queryBuilder` [Appeon.CoreService.Data.ISqlQueryBuilder](../../ISqlQueryBuilder/ISqlQueryBuilder.html)

一个SqlQueryBuilder实例，用户可以使用它覆盖TModel中预定义的静态的SQL检索规则，从而实现动态检索。

A SqlQueryBuilder instance which can be used to overwrite the static SQL query defined in a TModel class, so as to perform dynamic retrieval.

`parameters` System.Object[]

(Optional) One or more values that you want to use as retrieval arguments in the SQL SELECT statement defined in queryBuilder.

**Returns**

[Appeon.CoreService.Data.ILoadable&#60;TModel>](../../ILoadable/ILoadable.html)

返回ILoadable&#60;TModel>接口，可使用该接口的 Method进一步获取数据结果集，或者进行嵌套查询等操作。

Returns the ILoadable&#60;TModel> interface whose methods can be used to further obtain the data result set or perform data operations such as embedded queries.

### **Remarks**



### **Examples**





### **Applies to**

.NET Standard 

2.x