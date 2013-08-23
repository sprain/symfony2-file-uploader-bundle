Hochzytsreis is using Blueimp uploader based on the basic plugin implementation:
<https://github.com/blueimp/jQuery-File-Upload/wiki/Basic-plugin>

The original PunkAveFileUploaderBundle is not directed towards this kind of use. Several adjustments have been made for this implementation:

* In PunkAve/FileUploaderBundle/BlueImp/UploaderHandler.php the image_versions->thumbnail had to be uncommented (we don't need it)
* In PunkAve/FileUploaderBundle/BlueImp/UploaderHandler.php the upload result is being returned instead of echoed.
* All Header outputs have been disabled
* The exit at the end of FileUploader has benen uncommented.
* Also the javascript files in use are provided directly with the public resources and not being used from this bundle.

Original bundle:
<https://github.com/punkave/symfony2-file-uploader-bundle>