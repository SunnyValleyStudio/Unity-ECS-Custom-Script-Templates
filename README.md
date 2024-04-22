# Custom Script templates that you can use in your own ECS project

![image](https://github.com/SunnyValleyStudio/Unity-ECS-Custom-Script-Templates/assets/17239042/9beb0203-1ade-450d-96ae-9c06e7df701a)

Just add the **ScriptTemplates** folder to your **Assets** folder inside your Unity project. 

![image](https://github.com/SunnyValleyStudio/Unity-ECS-Custom-Script-Templates/assets/17239042/db8a224d-aa66-4930-b13c-aeb48428a57a)

<br>

## Naming Convention:
<p>81-ECS Script Templates__C# ECS Authoring-NewAuthoring.cs.txt

|Parameter | Description |
|-------------|-------------|
|"81" | Lower the number the higher the temolate will show up in the Create menu|
|"ECS Script Templates__C# ECS Authoring" | Path definition. Here the template will be in "Create -> ECS Script Templates" category and it will have a name "C# ECS Authoring" |
|"NewAuthoring.cs"| Name of the file that will be created in the Project tab in unity |
|".txt"| Tempalte needs to be saved as a Text file|

<br>

## Template Definition
```
public class #SCRIPTNAME# : MonoBehaviour
{

}

public class #SCRIPTNAME#Baker : Baker<#SCRIPTNAME#>
{
    public override void Bake(#SCRIPTNAME# authoring)
    {

    }
}
```

**#SCRIPTNAME#** - This will be swapped for the name that you gave to your script

<p>*To use those specific Script Templates make sure that you have [Entities package](https://docs.unity3d.com/Packages/com.unity.entities@1.0/manual/index.html) installed in yopur project
