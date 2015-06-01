# Ranged metadata

## Overall things to think about

* Implement processing of lowercase stuff in IO
* Modify tests to be generic across metadata slicing
* Getitem needs to handle all positional metadata, not just quality
* Implement metadata as a python dict
* Metadata equality whitelist and blacklist
* Add copy method to Sequence?
* Refactor Sequence.__getitem__
* Create pandas dataframe diff plugin for ipython

## Current todo

* Try to refactor complement in NucleotideSequence to not check _has_quality
  twice.
* Figure out if _set_quality is necessary (guessing it should not be)
* Tests to init metadata via different methods (dataframe vs dict etc)
* Sequence objects need to compare directly to string
* Test init metadata of different dtypes (float, etc)
* Replace internal part of _slices_from_iter with _index_to_slice
* tests that use getitem_empty_indices
* __repr__ for metadata
* _to should probably selectively update metadata


## Questions

* Should there be any sort of validation on metadata items?
