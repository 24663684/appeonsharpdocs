

## **IModelMapper.TrackUpdateRange&#60;TModel>(IEnumerable&#60;TModel> models) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个或者多个数据库表修改操作,将修改数据库表的数据缓存于TModel中。当IModelMapper.SaveChanges被调用时，一条或者多条SQL UPDATE statement 将用缓存在TModel中的数据以及被定义在TModel中的映射信息来产生，并执行。

Tracks one or more database table update operations. The data that will be updated to the database table is cached in TModel. When IModelMapper.SaveChanges is called, one or more SQL UPDATE statements will be first generated using the data cached in TModel and the mapping information defined in TModel, and then executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackUpdateRange<TModel>(IEnumerable<TModel> models);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standard.

**Parameters**

`models` System.Collections.Generic.IEnumerable&#60;TModel>

A Collection of TModel type, 用于修改一行或者多行记录。

A collection of TModel type used for updating one or multiple records.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### **Remarks**



### **Examples**



### **Applies to**

.NET Standard 

2.x