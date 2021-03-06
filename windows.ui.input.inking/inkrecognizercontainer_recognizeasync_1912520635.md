---
-api-id: M:Windows.UI.Input.Inking.InkRecognizerContainer.RecognizeAsync(Windows.UI.Input.Inking.InkStrokeContainer,Windows.UI.Input.Inking.InkRecognitionTarget)
-api-type: winrt method
-api-device-family-note: xbox
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<Windows.Foundation.Collections.IVectorView<Windows.UI.Input.Inking.InkRecognitionResult>> RecognizeAsync(Windows.UI.Input.Inking.InkStrokeContainer strokeCollection, Windows.UI.Input.Inking.InkRecognitionTarget recognitionTarget)
-->

# Windows.UI.Input.Inking.InkRecognizerContainer.RecognizeAsync

## -description
Performs handwriting recognition on one or more [InkStroke](inkstroke.md) objects.

## -parameters
### -param strokeCollection
The set of strokes on which recognition is performed.

### -param recognitionTarget
One of the values from the [InkRecognitionTarget](inkrecognitiontarget.md) enumeration.

## -returns
The results of the recognition as a collection of [InkRecognitionResult](inkrecognitionresult.md) objects.Each item in the collection represents a written word. For example, the string "this is a test" contains four words that are stored as a collection of four items.

## -remarks
Because [RecognizeAsync](inkmanager_recognizeasync_1262794931.md) does not automatically update the existing recognition results stored in the [InkManager](inkmanager.md), typically [UpdateRecognitionResults](inkmanager_updaterecognitionresults_1771366374.md) is called after [RecognizeAsync](inkmanager_recognizeasync_1262794931.md) has completed.

## -examples

## -see-also
[GetTextCandidates](inkrecognitionresult_gettextcandidates_1780889583.md), [Ink stroke recognition](http://msdn.microsoft.com/library/c2f3f3ce-737f-4652-98b7-5278a462f9d3), [Ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620308), [Simple ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620312), [Complex ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620314)