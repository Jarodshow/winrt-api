---
-api-id: M:Windows.Web.Http.HttpStreamContent.ReadAsBufferAsync
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperationWithProgress<Windows.Storage.Streams.IBuffer, ulong> ReadAsBufferAsync()
-->

# Windows.Web.Http.HttpStreamContent.ReadAsBufferAsync

## -description
Serialize the [HttpStreamContent](httpstreamcontent.md) to a buffer as an asynchronous operation.

## -returns
The object representing the asynchronous operation.

## -remarks
This operation will not block. The returned [IAsyncOperationWithProgress(IBuffer, UInt64)](../windows.foundation/iasyncoperationwithprogress_2.md) object will complete after all of the content has been written to the buffer.

The [HttpStreamContent](httpstreamcontent.md) class can be used to stream content that might be of arbitrary length. The [ReadAsBufferAsync](httpstreamcontent_readasbufferasync_1151439480.md) method will fail if all of the [HttpStreamContent](httpstreamcontent.md) can't fit in memory since this method requires the entire content to be buffered in memory first.

## -examples

## -see-also
