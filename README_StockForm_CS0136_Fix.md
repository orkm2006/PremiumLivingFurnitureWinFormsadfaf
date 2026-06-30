# StockForm CS0136 and Sidebar Warning Fix

## Fixed

1. StockForm.cs
   - Fixed CS0136 caused by declaring `selectedProduct` more than once in the same method scope.
   - Renamed pattern variables to:
     - finishedProductLookup
     - fallbackProductLookup
     - nonProductTypeLookup

2. MainForm.cs
   - Fixed CS8604 warning by checking `e.Control != null` before calling `HookMouseWheel(e.Control)`.

## Apply

1. Replace StockForm.cs.
2. Replace MainForm.cs if you want to remove the CS8604 warning.
3. Clean Solution.
4. Rebuild Solution.
