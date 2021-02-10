# 3DTILES_metadata

This extension provides a formal mechanism for attaching application-specific metadata to various components of 3D Tiles.

## Changelog

* [**Version 0.0.0**](0.0.0/README.md) November 6, 2020
    * Initial draft
* [**Version 1.0.0**](1.0.0/README.md) [TODO: Date]
    * Changes to properties
      * Removed `FLOAT16` type
      * Removed `BLOB` type and `blobByteLength` property
      * Removed `stringByteLength` property
      * Added optional `semantic` property
      * Added enum support. Added `ENUM` to `type` and `componentType` and added `enumType` property.
    * Changes to `3DTILES_metadata` extension object
      * Added `schema` which contains `classes` and `enums`
      * Added `groups` which contain metadata about groups of content. Contents are assigned to groups with the `3DTILES_metadata` content extension.
      * Added `statistics` which provide aggregate information about select properties within a tileset.
    * Added tile metadata. A tile may specify its class and property values with the `3DTILES_metadata` tile extension object.
    * Added support for tile metadata in the `3DTILES_implicit_tiling` extension. Tile metadata may be provided for each subtree in binary.