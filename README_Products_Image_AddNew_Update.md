# Products Add New Image Update

## What changed

- Products > Add New now opens a dedicated ProductForm.
- ProductForm supports selecting a product image.
- The selected image is previewed before saving.
- When saved, the image is copied to the application folder under `ProductImages/`.
- The product record stores the relative image path in `Products.ImagePath`.
- ProductForm automatically adds the `ImagePath` column to the Products table if it does not exist.

## Files included

- MainForm.cs
- ProductForm.cs

## Apply

1. Replace MainForm.cs.
2. Add ProductForm.cs to the Visual Studio project.
3. Clean Solution.
4. Rebuild Solution.
5. Open Products > Add New.

## Notes

Supported image files: JPG, JPEG, PNG, BMP, GIF.
