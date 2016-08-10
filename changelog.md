
# Change Log

Ark adheres to [semantic versioning][semver].

[semver]: http://semver.org



## 2.1.0

* This release is identical to 2.0.0. Incrementing the minor version resolves a packaging issue caused by misnamed beta releases.



## 2.0.0

* Major release containing breaking changes to the theme and plugin API.

* Numerous enhancements to the application's command line interface.

* New default theme, `phoenix`.

* Themes can now bundle plugins in a `code` directory.

* Command line arguments are now parsed *before* extensions are loaded.

* The site configuration file has been renamed from `config.py` to `ark.py`.

* Ark no longer requires an empty `.ark` sentinel file to locate the home directory. Instead it will use the presence of *either* an `ark.py` file *or* both `src` and `out` directories.

* The preprocessor system for parsing record metadata (e.g. YAML file headers) has been replaced by a single filter hook, `file_text`.

* A bundled `breadcrumbs` plugin replaces and enhances the functionality of the old `trail` page attribute.