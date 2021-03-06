---
-api-id: T:Windows.UI.Xaml.Automation.Peers.RichEditBoxAutomationPeer
-api-type: winrt class
---

<!-- Class syntax.
public class RichEditBoxAutomationPeer : Windows.UI.Xaml.Automation.Peers.FrameworkElementAutomationPeer, Windows.UI.Xaml.Automation.Peers.IRichEditBoxAutomationPeer
-->

# Windows.UI.Xaml.Automation.Peers.RichEditBoxAutomationPeer

## -description
Exposes [RichEditBox](../windows.ui.xaml.controls/richeditbox.md) types to Microsoft UI Automation.

## -remarks
The Windows Runtime  [RichEditBox](../windows.ui.xaml.controls/richeditbox.md) class creates a new [RichEditBoxAutomationPeer](richeditboxautomationpeer.md) as its [OnCreateAutomationPeer](../windows.ui.xaml/uielement_oncreateautomationpeer.md) definition. Derive your automation peer from [RichEditBoxAutomationPeer](richeditboxautomationpeer.md) if you are deriving a custom class from [RichEditBox](../windows.ui.xaml.controls/richeditbox.md) and want to add automation support for additional features that you enabled in your custom class. Then override [OnCreateAutomationPeer](../windows.ui.xaml/uielement_oncreateautomationpeer.md) so that it returns your custom peer.

### Default peer implementation and overrides in **RichEditBoxAutomationPeer**

[RichEditBoxAutomationPeer](richeditboxautomationpeer.md) has overrides of **Core** methods such that the associated [AutomationPeer](automationpeer.md) methods provide peer-specific information to a Microsoft UI Automation client.

+ [GetPattern](automationpeer_getpattern.md) reports pattern support for [TextPattern](http://msdn.microsoft.com/library/ddcf7ecd-7ed2-4b57-82a7-c7e1608dbfa1), but see "TextPattern support" in this topic for more info.
+ [GetClassName](automationpeer_getclassname.md) returns "RichEditBox".
+ [GetAutomationControlType](automationpeer_getautomationcontroltype.md) returns [AutomationControlType.Edit](automationcontroltype.md).
+ [IsControlElement](automationpeer_iscontrolelement.md) returns **true**.
<!--not sure how this gets set cannot see in the partial cpp-->
The peer also has other behaviors that are provided by the base [FrameworkElementAutomationPeer](frameworkelementautomationpeer.md) class. For more info, see "Base implementation in FrameworkElementAutomationPeer" section of [Custom automation peers](http://msdn.microsoft.com/library/aa8da53b-fe6e-40ac-9f0a-cb09637c87b4).

### TextPattern support

 [RichEditBoxAutomationPeer](richeditboxautomationpeer.md) supports the **TextPattern**  Microsoft UI Automation pattern. The support for this pattern is implemented as native code by the peer, so you won't see public API for the [RichEditBoxAutomationPeer](richeditboxautomationpeer.md) peer class that exposes the pattern implementation for extension. And you won't see [ITextRangeProvider](../windows.ui.xaml.automation.provider/itextrangeprovider.md) and the similar managed interfaces in the [RichEditBoxAutomationPeer](richeditboxautomationpeer.md) inheritance. But Microsoft UI Automation clients can use the **TextPattern** pattern implemented by this peer and call its native API surface.


<!--<p  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">specifics of the <xref targtype="iface" rid="winauto.uiauto_IUIAutomationTextPattern">TextPattern</xref> implementation .... not documented</p>-->

## -examples

## -see-also
[RichEditBox](../windows.ui.xaml.controls/richeditbox.md), [FrameworkElementAutomationPeer](frameworkelementautomationpeer.md), [Custom automation peers](http://msdn.microsoft.com/library/aa8da53b-fe6e-40ac-9f0a-cb09637c87b4)