# CSS Manifests Lab

## Objectives

1. Create CSS Manifest Files
2. Require CSS Files in Manifests with Sprocket Directives
3. Include CSS Manifest Files in Layouts

## Outline

Give them a rails app with a few css files in random asset paths like app/assets and vendor/assets and one file in the wrong place (like lib/assets/stylesheets) so they also have to move the file (or even if you provide a hint keep the file there just add lib/assets/stylesheets to the asset paths in the initializer. you can individually test for this too by looking at Rails.application.assets.paths to see that directory included). Delete the manifest file. Give them two layouts, an application layout and an admin layout.

Tell them to create an application manifest with 3 of the 5 css files put in random places. Then they need to load that manifest into the application layout.

Then they should do the same (2 new CSS files, 1 from the application manifest too so that they know CSS files don't need to be unique to one manifest vs the other) for the admin manifest and admin layout.

the admin layout should also stylesheet_link_tag another random CSS file that isn't in the manifest but is in app/assets so they know how to include a non manifested CSS file.
