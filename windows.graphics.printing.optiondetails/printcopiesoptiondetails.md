---
-api-id: T:Windows.Graphics.Printing.OptionDetails.PrintCopiesOptionDetails
-api-type: winrt class
---

<!-- Class syntax.
public class PrintCopiesOptionDetails : Windows.Graphics.Printing.OptionDetails.IPrintNumberOptionDetails, Windows.Graphics.Printing.OptionDetails.IPrintOptionDetails
-->

# Windows.Graphics.Printing.OptionDetails.PrintCopiesOptionDetails

## -description
Represents the option for the number of printed copies.

## -remarks
Here is a JavaScript code snippet that shows how to retrieve the object:





```javascript
//  Retrieve the advanced Print Task Options
var printDetailedOptions = 
     Windows.Graphics.Printing.OptionDetails.PrintTaskOptionDetails.getFromPrintTaskOptions(printTask.options);

// get the object
var printCopiesOptionDetails = 
     printDetailedOptions.options.lookup(Windows.Graphics.Printing.StandardPrintTaskOptions.copies);
```



## -examples

## -see-also