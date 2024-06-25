# Release Keys

Realease keys are a specifically created to allow a remote documentation to a specific release. While a release is a specific analysis at a certain point in time, the structure (SBOM) of this solution will not change anymore. The idea of a release key is to create an API Key that has the single purpose to associate a specific document with a released software.

Thus this key will not allow anything else than calling the TrustSource API to pull any of the following documents:

- SBOM
- Notice File
- CSAF2.0 VEX

The prerequisite to create a Release key is to have a 