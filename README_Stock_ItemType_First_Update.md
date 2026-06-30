# Stock Add New Item Type First Update

## What changed

- Stock > Add New now opens a dedicated `StockForm`.
- The user must select `Item Type` first.
- `Product` selection is disabled until `Item Type` has been selected.
- The form still saves normal Stock fields:
  - ItemCode
  - ItemType
  - ProductId, optional
  - ItemName
  - Warehouse
  - Quantity
  - ReorderPoint
  - LastUpdated
- Existing stock status calculation still runs through `Database.AddRecord("Stock", ...)`.

## Files included

- MainForm.cs
- StockForm.cs

## Apply

1. Replace `MainForm.cs`.
2. Add `StockForm.cs` to the project.
3. Clean Solution.
4. Rebuild Solution.
5. Open Stock > Add New and test the new order.
