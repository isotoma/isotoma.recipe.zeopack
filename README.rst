Advanced zeopack recipe
=======================

The built-in zeopack component of the various plone server recipes is great,
but we've got a couple of gaps:

 * Before we started using zeopack we are a custom packer that would rotate the
   backups made, allowing us to keep a few days of backups of our Data.fs.  We
   missed it.

 * There isn't a zeopack-all to pack all your storages.

 * You can't control pack-days from the command line so you can't have
   different packing preferences per backend.

This recipe can pack all storages configured using your ``zeoserver`` and
``filestorage`` recipes.

