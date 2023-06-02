# xnat_mr_bvalue_fix
Plugin to fix the B-value issue with XNAT uploads.

## The issue
XNAT adds the B-values, obtained via DICOM metadata, to its database. However for large numbers of B-vectors, this exceeds the allocated database field size and results in an import error.

## What this plugin does
This plugin stops XNAT from obtaining the B-vector data for storage in its database, but still leaves it in the DICOM metadata.

