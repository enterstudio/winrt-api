---
-api-id: T:Windows.Media.PlayTo.PlayToSourceRequestedEventArgs
-api-type: winrt class
---

<!-- Class syntax.
public class PlayToSourceRequestedEventArgs : Windows.Media.PlayTo.IPlayToSourceRequestedEventArgs
-->

# Windows.Media.PlayTo.PlayToSourceRequestedEventArgs

## -description
Provides information about the [SourceRequested](playtomanager_sourcerequested.md) event.

## -remarks
<!--{annotation author="v-shawja" time="1/27/2012 12:44:35 PM"}In the following sentence, I formatted PlayToSourceRequestedEventArgs as a class, but please provide the correct targtype and rid attributes.-->
You use the [SourceRequest](playtosourcerequestedeventargs_sourcerequest.md) property of the  class to pass media from your application to Play To during the [SourceRequested](playtomanager_sourcerequested.md) event.

For an example of how to use Play To in an application, see [Quickstart: Using Play To in applications (JavaScript)](XREF:TODO:m_playto.using_playto_in_applications) or [PlayReady DRM](http://msdn.microsoft.com/library/dd8ffa8c-dff0-41e3-8f7a-345c5a248fc2).

## -examples


> [!div class="tabbedCodeSnippets"][!code-cs[SourceRequested](../windows.media.playto/code/PlayTo_Reference/csharp/MainPage.xaml.cs#SnippetSourceRequested)][!code-js[SourceRequested](../windows.media.playto/code/PlayTo_Reference/javascript/default.js#SnippetSourceRequested)][!code-vb[SourceRequested](../windows.media.playto/code/PlayTo_Reference/vbnet/MainPage.xaml.vb#SnippetSourceRequested)]

## -see-also
[SourceRequested](playtomanager_sourcerequested.md), [Play To sample](http://go.microsoft.com/fwlink/p/?linkid=245166), [PlayToReceiver sample](http://go.microsoft.com/fwlink/p/?linkid=245167), [Media Server sample](http://go.microsoft.com/fwlink/p/?linkid=245168)
