---
layout: post
title: Appearance of WPF AutoComplete | Syncfusion
description: Learn here about how to set the different style of theme to the Syncfusion WPF AutoComplete control.
platform: wpf
control: AutoComplete
documentation: ug
---

# Appearance of WPF AutoComplete

The Appearance of the AutoComplete control can be changed using the VisualStyle property. The following styles are supported by AutoComplete control.

* Blend
* Office2003
* Office2007Blue
* Office2007Black
* Office2007Silver
* ShinyBlue
* ShinyRed
* SyncOrange
* VS2010
* Metro
* Transparent 

The following code example illustrates how different visual styles can be applied to the control.

{% tabs %}
{% highlight xaml %}

<syncfusion:AutoComplete Height="25" Width="200" syncfusion:SkinStorage.VisualStyle="Office2007Blue"/>

{% endhighlight %}

{% highlight c# %}

SkinStorage.SetVisualStyle(autoComplete, "Office2007Blue");

{% endhighlight %}
{% endtabs %}

![Set Windows theme to WPF AutoComplete](Appearance_images/Appearance_img1.png)

Windows7
{:.caption}

![Set Blend theme to WPF AutoComplete](Appearance_images/Appearance_img2.png)

Blend
{:.caption}

![Set Office2007Blue theme to WPF AutoComplete](Appearance_images/Appearance_img3.png)

Office2007Blue
{:.caption}

![Set Office2007Black theme to WPF AutoComplete](Appearance_images/Appearance_img4.png)

Office2007Black
{:.caption}

![Set Office2007Silver theme to WPF AutoComplete](Appearance_images/Appearance_img5.png)

Office2007Silver
{:.caption}

![Set Office2003 theme to WPF AutoComplete](Appearance_images/Appearance_img6.png)

Office2003
{:.caption}

![Set ShinyRed theme to WPF AutoComplete](Appearance_images/Appearance_img7.png)

ShinyRed
{:.caption}

![Set ShinyBlue theme to WPF AutoComplete](Appearance_images/Appearance_img8.png)

ShinyBlue
{:.caption}

![Set SyncOrange theme to WPF AutoComplete](Appearance_images/Appearance_img9.png)

SyncOrange
{:.caption}

![Set Metro theme to WPF AutoComplete](Appearance_images/Appearance_img10.png)

Metro
{:.caption}

![Set the Transparent theme to AutoComplete](Appearance_images/Appearance_img11.png)

Transparent
{:.caption}

## Show the shadow effect

You can show the shadow effect of AutoComplete by using [DropShadowEffect](https://docs.microsoft.com/en-us/dotnet/api/system.windows.media.effects.dropshadoweffect?view=netcore-3.1). You can also set the distance between the control and shadow by using [ShadowDepth](https://docs.microsoft.com/en-us/dotnet/api/system.windows.media.effects.dropshadoweffect.shadowdepthproperty?view=netcore-3.1) property.

Refer the below code for your reference.

{% tabs %}

{% highlight XAML %}

<syncfusion:AutoComplete Height="30" Width="150" Text="AutoComplete">
    <syncfusion:AutoComplete.Effect>
        <DropShadowEffect ShadowDepth="10" Color="LightGray" Opacity="2" />
    </syncfusion:AutoComplete.Effect>
</syncfusion:AutoComplete>

{% endhighlight %}

{% highlight C# %}

AutoComplete autoComplete = new AutoComplete();
autoComplete.Height = 30;
autoComplete.Width = 150;
autoComplete.Text = "AutoComplete";
DropShadowEffect shadowEffect = new DropShadowEffect();
shadowEffect.ShadowDepth = 10;
shadowEffect.Color = Colors.LightGray;
shadowEffect.Opacity = 2;
autoComplete.Effect = shadowEffect;
grid.Children.Add(autoComplete);

{% endhighlight %}

{% endtabs %}

![Show the shadow effects of WPF AutoComplete](Appearance_images/wpf-autocomplete-shadow.png)
