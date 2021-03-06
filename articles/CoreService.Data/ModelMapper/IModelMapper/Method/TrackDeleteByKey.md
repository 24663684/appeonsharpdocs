

## **IModelMapper.TrackDeleteByKey&#60;TModel>(params object[] parameters) Method**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">
<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

追踪一个数据库表的按主键进行删除的操作， 用传入的主键值以及被定义在TModel中的映射信息来产生一条SQL DELETE statement。当IModelMapper.SaveChanges被调用时，该SQL DELETE statement 将被执行。

Tracks a database table delete operation by primary key. A SQL DELETE statement will be generated using the primary key value(s) and the mapping information defined in TModel. When IModelMapper.SaveChanges is called, the SQL DELETE statement will be executed.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
  public IModelMapper TrackDeleteByKey<TModel>(params object[] parameters);
```

**Type Parameters**

`TModel`

The type of a model class that conforms to the Appeon standard.

**Parameters**

`parameters` System.Object[]

(Optional) One or more primary key values that you want to use as arguments in the SQL DELETE statement.

**Returns**

[Appeon.CoreService.Data.IModelMapper](../../IModelMapper/IModelMapper.html)

返回一个IModelMapper接口，可以使用该接口继续使用当前ModelMapper实例执行其他 Method。

Returns an IModelMapper interface, which can be used for executing other methods with the current ModelMapper instance.

### Remarks

**Cascade Delete**

如需同时删除主表和明细表中关联的记录，可在TModel中定义主表和明细表的级联删除规则，具体参考关于ModelEmbeddedAttrubute的说明。

If the record in the master table and its associated records in the detail table must be deleted at the same time, you can define the cascade deletion rule for the master and the detail tables in TModel. Refer to the [ModelEmbedded](../../ModelAttribute/Property/ModelEmbeddedAttribute/ModelEmbeddedAttribute.html) attribute for more.

### **Examples**



### **Applies to**

.NET Standard 

2.x