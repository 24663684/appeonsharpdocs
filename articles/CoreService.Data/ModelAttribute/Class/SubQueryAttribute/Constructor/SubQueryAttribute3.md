## **SubQueryAttribute.SubQueryAttribute(string name, Type modelType, string selectName) Constructor**

**.NET Standard 2.x |**  <a href="javascript:void(0)" class="dropdown">Current version (0.5.0-alpha) <img src="~/images/dropdown.png"/></a>

<div class="otherversions"  value="versdiv">

<a href="javascript:void(0)">0.5.0-alpha</a>

<a href="javascript:void(0)">0.5.1-alpha(current)</a>

</div>

Initializes a new instance of the SubQueryAttribute class.

 **Namespace:** Appeon.CoreService.Data

 **Assembly:** Appeon.CoreService.Data.dll

### **Syntax**

```c#
   public SubQueryAttribute(string name, Type modelType, string selectName)
```

**Parameters**

`name` System.String

The name of the subquery.

`modelType` System.Type

The type of the model that represents the subquery.

`selectName` System.String

Select Name (SqlSelectAttribute.SelectName) predefined in modelType which can switch the SELECT clause.

### **Remarks**





### **Applies to**

.NET Standard 

2.x