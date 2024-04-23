# :muscle: Custom Script templates that you can use in your own ECS project 

![image](https://github.com/SunnyValleyStudio/Unity-ECS-Custom-Script-Templates/assets/17239042/9beb0203-1ade-450d-96ae-9c06e7df701a)

Just add the **ScriptTemplates** folder to your **Assets** folder inside your Unity project. 

![image](https://github.com/SunnyValleyStudio/Unity-ECS-Custom-Script-Templates/assets/17239042/8a1f463e-8112-40be-908a-370dda83b2d7)

<br>

## :star: Naming Convention:
<p>81-ECS Script Templates__C# ECS Authoring-NewAuthoring.cs.txt

|Parameter | Description |
|-------------|-------------|
|"81" | Number defining the order in the Create menu. The lower the value the higher the template will appear |
|"ECS Script Templates__C# ECS Authoring" | Path definition. Here the template will be in "Create -> ECS Script Templates" category and it will have a name "C# ECS Authoring" |
|"NewAuthoring.cs"| Name and the extension of the file that will be created in the Project tab in unity |
|".txt"| Tempalte needs to be saved as a Text file|

<br>

## :book: Template Definition
```
using Unity.Entities;
using UnityEngine;

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

**#SCRIPTNAME#** - This will be swapped for the name that you gave to your script. We can add to it prefix or a suffix like I do with "#SCRIPTNAME#Baker"
<p>*To use those specific Script Templates make sure that you have [Entities package](https://docs.unity3d.com/Packages/com.unity.entities@1.0/manual/index.html) installed in yopur project

<br><br>

## :sparkling_heart: Feeling generous?
:arrow_forward:Help me out by **subscribing** to my YT channel https://www.youtube.com/@SunnyValleyStudio :hearts:
<br>
:arrow_forward:You can also support what I do [through Patreon](https://www.patreon.com/sunnyvalleystudio) :hearts:
