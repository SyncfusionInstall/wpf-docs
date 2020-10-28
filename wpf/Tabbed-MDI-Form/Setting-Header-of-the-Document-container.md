---
layout: post
title: Setting Header of the Document container| DocumentContainer | Wpf | Syncfusion
description: setting header of the document container
platform: wpf
control: DocumentContainer
documentation: ug
---

# Setting Header of the DocumentContainer

Using the `Header` property, user can set the header for the DocumentContainer elements. Use the following code snippet, to set the header for the DocumentContainer element.


{% highlight xaml %}

<!-- Adding Document Container -->

<syncfusion:DocumentContainer Name="DocContainer"  Mode="MDI">

<FlowDocumentScrollViewer x:Name="flow" syncfusion:DocumentContainer.Header="Features">

</FlowDocumentScrollViewer>

…....

…....

</syncfusion:DocumentContainer>

{% endhighlight %}

### Setting header programmatically

Header of the DocumentContainer elements can be set by `SetHeader` method. 

{% tabs %}

{% highlight C# %}

//Set the Header of the DocumentContainer

DocumentContainer.SetHeader(flow, "Features");

{% endhighlight %}

{% endtabs %}

![](Setting-Header-of-the-Document-container_images/Setting-Header-of-the-Document-container_img1.jpeg)


