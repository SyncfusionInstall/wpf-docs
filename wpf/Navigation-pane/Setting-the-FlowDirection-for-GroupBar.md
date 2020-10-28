---
layout: post
title: Setting the FlowDirection for GroupBar| GroupBar | Wpf | Syncfusion
description: setting the flowdirection for groupbar
platform: wpf
control: GroupBar
documentation: ug
---

# Setting the FlowDirection for GroupBar

Flow Direction of the GroupBar is set by using the FlowDirection property. 

### Property Table

<table>
<tr>
<th>
Property</th><th>
Description</th></tr>
<tr>
<td>
FlowDirection</td><td>
Sets the flow direction for the GroupBar control. The options provided are as follows.* LeftToRight* RightToLeft</td></tr>
</table>



Use the following code snippet to set this property.

{% tabs %}
{% highlight xaml %}
<!-- Adding GroupBar that has flow direction as left to right -->
<syncfusion:GroupBar Height="300" Width="230" Name="groupBar" FlowDirection="RightToLeft">
<!-- Adding GroupBarItem -->
<syncfusion:GroupBarItem Name="groupBarItem1" HeaderImageSource="Label.gif" Header="General">
  <!-- Adding content for GroupBar item using GroupView --> 
  <syncfusion:GroupView Name="groupView" IsListViewMode="True"> 
  <syncfusion:GroupViewItem Text="List View"/>   
  <syncfusion:GroupViewItem Text="Show ContextMenu"/>  
  <syncfusion:GroupViewItem Text="Show ToolTip"/> 
  </syncfusion:GroupView></syncfusion:GroupBarItem>
  <!-- Adding GroupBarItem -->
  <syncfusion:GroupBarItem HeaderImageSource="Tasks.png" Name="groupBarItem2" Header="Visual Mode">
  <!-- Adding content for GroupBar item using GroupView -->
  <syncfusion:GroupView>   
  <syncfusion:GroupViewItem Text="Default"/> 
  <syncfusion:GroupViewItem Text="Multiple Expansion"/>  
  <syncfusion:GroupViewItem Text="StackMode"/>
  </syncfusion:GroupView></syncfusion:GroupBarItem>
  <!-- Adding GroupBarItem -->
  <syncfusion:GroupBarItem HeaderImageSource="Notes.png" Name="groupBarItem3" Header="State Persistence">  
  <!-- Adding content for GroupBar item using GroupView -->  
  
  <syncfusion:GroupView>  
  <syncfusion:GroupViewItem Text="Save State"/>  
  <syncfusion:GroupViewItem Text="Load State"/>  
  <syncfusion:GroupViewItem Text="Reset State"/>  
  </syncfusion:GroupView></syncfusion:GroupBarItem>
  </syncfusion:GroupBar>
  {% endhighlight %}

{% highlight C# %}
// Setting flow direction as RightToLeft
groupBar.FlowDirection = FlowDirection.RightToLeft;
 {% endhighlight %} 
{% endtabs %}


