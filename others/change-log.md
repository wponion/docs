# Change Log

## Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),

and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.5.3.2](https://github.com/wponion/wponion/releases/tag/1.5.3.2) - 23/07/2020

### Added

* DB Save Hook Support For Settings & Network Settings Module
* `set_unique` function in **Unique** Trait
* `set_module` function in **Module** Trait
* new `object` Trait created
* Custom Save Handler For Every Module.
* **Action :** `wponion/metabox/render/before`
* **Action :** `wponion/metabox/render/{$this->unique()}/before`
* **Action :** `wponion/metabox/render/{$this->unique()}/after`
* **Action :** `wponion/metabox/render/after`
* Custom Class Option In Admin Page Module
* Notification Bubble Support In Admin Page Module
* Menu Separator Support In Admin Page Module

### Fixed

* Taxonmy Register Issue . fixed by changing `$this->taxonomy` to `$this->unique()`
* **CSS** Tab layout `z-index`
* Ajax issue with metabox saving

### Changed

* Bump [@wordpress/hooks](https://github.com/WordPress/gutenberg/tree/HEAD/packages/hooks) from `2.8.0` to `2.9.0`
* Bump \[@popperjs/core\] from `2.4.2` to `2.4.4`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `6.2.3` to `6.2.5`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.15.1` to `9.17.0`
* Bump [css-checkbox-library](https://github.com/hunzaboy/CSS-Checkbox-Library) from `1.5.1` to `1.5.2`

### Removed

* Deleted local function calls added by mistake

## [1.5.3.1](https://github.com/wponion/wponion/releases/tag/1.5.3.1) - 23/06/2020

### Fixed

* Custom Template Tags Not Working In Selectbox

## [1.5.3](https://github.com/wponion/wponion/releases/tag/1.5.3) - 17/06/2020

### Added

* Option To Customize Page's Browser Title

### Fixed

* Select Ajax Query Args Not Working Fields Outside WPOnion Module 

### Changed

* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.14.4` to `9.15.1`
* WPOnion Core Assets CDN Version To `1.4`

## [1.5.2](https://github.com/wponion/wponion/releases/tag/1.5.2) - 14/06/2020

### Fixed

* [Fatal Error When Using Along Side Elementor Plugin](https://github.com/wponion/wponion/issues/252)

### Changed

* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.14.0` to `9.14.4` \#250 
* Bump \[@popperjs/core\] from `2.4.0` to `2.4.2` \#251 

## [1.5.1](https://github.com/wponion/wponion/releases/tag/1.5.1) - 06/06/2020

### Changed

* `wponion_icon` function now can handle image link

### Fixed

* Performace Fix in Storage Interface.

## [1.5](https://github.com/wponion/wponion/releases/tag/1.5) - 06/06/2020

### Added

* **Hook Priority** option in taxonomy
* `WPONION_PLUGIN_FILE` constant in plugin file.
* Deprecation handlers for \(Function,Actions,Filters\)
* Nested Array Support for `Class_Options` Trait
* Option to have external links in **Admin Page** Module
* Changes Browser URL when click tab in settings page \(useful if everything loads in a single page\)
* is empty check with array `wponion_is_array`
* Created Storage Handlers which interacts with wordpress DB.
* **Action**   :  "wponion/{$this-&gt;module\(\)}/get/before"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/{$this-&gt;unique\(\)}/get/before"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/{$this-&gt;unique\(\)}/get/after"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/get/after"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/save/before"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/{$this-&gt;unique\(\)}/save/before"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/{$this-&gt;unique\(\)}/save/after"
* **Action**   :  "wponion/{$this-&gt;module\(\)}/save/after"
* **Filters**  :  "wponion/{$this-&gt;module\(\)}/get/values"
* **Filters**  :  "wponion/{$this-&gt;module\(\)}/{$this-&gt;unique\(\)}/get/values"
* **Filters**  :  "wponion/{$this-&gt;module\(\)}/save/values"
* **Filters**  :  "wponion/{$this-&gt;module\(\)}/{$this-&gt;unique\(\)}//save/values"
* **Function** :  `wponion_cast_array`
* **Function** :  `wponion_has_column_class`
* **Function** :  `wponion_parse_args_mixed`
* **Function** :  `wponion_parse_args_forced_values`
* **Function** :  `wponion_cast_array`
* **Function** :  `wponion_define`
* **Function** :  `wponion_is_defined`
* **Function** :  `wponion_is_set`
* **Function** :  `wponion_is_version`

### Fixed

* [\#233  `theme` arg in Taxonomy Module produces error if theme is not `wp_modern`](https://github.com/wponion/wponion/issues/233)
* CSS fix for switcher field.
* Admin Notice Database Fetching Issue.
* Assets Loading issue in `Page Actions` Module
* Improved Performance.

### Changed

* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.12` to `9.14.0`
* Reworked Admin Notice Module and changed all function names to match wponion format
* Moved `Setup` folder from `core/` to `/`
* Moved Some Internal Options Arg to data folder
* Moved `builder` Files From Root To `includes/`
* Moved `Templates` From Root To `includes/`
* Moved `module-fields` from Root to `includes/`
* Moved `fields` from Root to `includes/`
* Moved `integrations` from `core/` to `includes/`
* Cleanup done for `core/helpers` and moved to `core/functions`
* Renamed Certain Files With Proper Prefix
* 24+ **Deprecated Action**
* 16+ **Deprecated Filters**
* **Deprecated Function** `wpo_help` use `wponion_tooltip`
* **Deprecated Function** `wponion_validate_bool_val` use `wponion_is_bool_val`
* **Deprecated Function** `wponion_get_field_class_remap` use `wponion_field_class_remaps`
* **Deprecated Function** `wponion_get_registry_instance`
* **Deprecated Function** `wponion_is` use `wponion_is_instance`
* **Deprecated Function** `wponion_field_debug` use `wponion_is_field_debug`
* Refactor for all modules and rearranged in its proper folder.
* Base Unique Returns Unique Value if Base Unique not exists.

### Removed

* Autoloader's Instance
* `if(class_exists())`,`if(trait_exists())`,`if(interface_exists())` checks

## [1.4.6](https://github.com/wponion/wponion/releases/tag/1.4.6) - 06/05/2020

### Fixed

* WooCommerce Localizer Issue \(Not Properly Loading\)
* Accordion Style In WC Metabox
* Tab Dependency Issue
* [Content Field Warning \#234](https://github.com/wponion/wponion/issues/234) 

### Added

* All Modules in WPOnion Can Provide An Option To Load Custom Assets via `"assets" => "your-asset"` in module argument.
* Function `->section` it can be used instead of `->container` inside tab field
* **ACTION** `wponion_query_database`
* **ACTION** `wponion_{module_slug}_db_save_before`
* **ACTION** `wponion_{module_slug}_db_save_after`
* **FILTER** `wponion_ajax_wp_query_results`
* **FILTER** `wponion_wp_query_result`
* **FILTER** `wponion_query_args`
* **NEW** `add_field` Method In Builder 
* `wponion-inline-dependency` option 
* `image_sizes` WP Query Data Option.
* `user_roles` WP Query Data Option.
* `capabilities` WP Query Data Option.

### Changed

* **Deprecated** `field` Method In Builder 
* **Deprecated** `->container` inside tab field
* Swticher style prefix changed from `ckbx-` to `wpock-`
* Moved custom asset loader functions from admin-page module to `wponion_load_asset`
* Rearranged Arguments for `wpo_user_meta`,`wpo_post_meta`
* Bump [css-checkbox-library](https://github.com/hunzaboy/CSS-Checkbox-Library) from `1.4.0` to `1.5.1`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `6.2.0` to `6.2.3` 
* Bump \[@popperjs/core\] from `2.3.3` to `2.4.0`
* Bump \[jquery\] from `3.4.1` to `3.5.1`

### Removed

* `load_from_existing` from builder
* `.wponion-framework` prefxed style changed from \(`.wponion-framework.wponion-module-settings`\) to \(`.wponion-module-settings`\) in css
* `.wponion-framework` prefxed style changed from \(`.wponion-framework.wponion-element-accordion`\) to \(`.wponion-element-accordion`\) in css

## [1.4.5.3](https://github.com/wponion/wponion/releases/tag/1.4.5.3) - 22/04/2020

### Fixed

* Bootstrap Style issue with Porto Theme \#221 

### Changed

* Bump [@wordpress/hooks](https://github.com/WordPress/gutenberg/tree/HEAD/packages/hooks) from `2.7.0` to `2.8.0`
* Bump [WPOnion Icons](https://icons.wponion.com) from `1.0.0' to`1.0.3\`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `6.1.1` to `6.2.0`
* Bump \[@wponion/flexboxgrid2 \]from `1.0.1` to `1.0.2`
* Bump \[@popperjs/core\] from `2.3.2` to `2.3.3`
* Moved Alerts CSS From normal to wpo- prefixed
* Moved Jumbotron css from normal to wpo- prefixed
* Moved table css from normal to wpo- prefixed
* Combined Multiple media query for the same style into 1.

### Removed

* `.wponion-element` prefix for each element's style remvoed to reduce css file size
* `wponion-plugins.css` file combined to `wponion-base.css` and removed.

## [1.4.5.2](https://github.com/wponion/wponion/releases/tag/1.4.5.2) - 14/04/2020

### Changed

* Improved Settings Page / Metabox Menu Navtion Easy.
* Improved PHP Documentation.
* Bump \[@popperjs/core\] from `2.2.1` to `2.3.2`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.9` to `9.10.12`

### Fixed

* `select2` CSS Bug Fixed.
* `query_args` in `\WPO\Container` callback fixed.

### Removed

* Deleted All `\WPO\Field`  Get method's comments.

## [1.4.5.1](https://github.com/wponion/wponion/releases/tag/1.4.5.1) - 06/04/2020

### Changed

* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.8` to `9.10.9`
* Bump [popper.js](https://popper.js.org) from `2.1.1` to `2.2.1`
* Bump [WPOnion Icons](https://icons.wponion.com) from `1.0.1` to `1.0.2`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `6.1.0` to `6.1.1`

## [1.4.5](https://github.com/wponion/wponion/releases/tag/1.4.5) - 02/04/2020

### Fixed

* Multiple Ajax Request when using CTRL+S
* Warning When Direct CSS Added `$field->parse('color:red');` fixed.
* Updated WPOnion to use `wp_nav_menu_item_custom_fields` hook instead of custom walker if wordpress version is 5.4 =&gt;

### Changed

* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.7` to `9.10.8`
* Bump [WPOnion Icons](https://icons.wponion.com) from `1.0.0' to`1.0.1\`
* **button** Field type changed to UI
* **modal** Field type changed to UI
* **wp\_list\_table** Field type changed to UI

## [1.4.4](https://github.com/wponion/wponion/releases/tag/1.4.4) - 30/03/2020

### Added

* Option to set custom css style per field `$field->css('font-size:12px;')`

### Fixed

* Responsive Field styles.

### Changed

* Column Layout changed for all field types
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.6` to `9.10.7`

## [1.4.3](https://github.com/wponion/wponion/releases/tag/1.4.3) - 26/03/2020

### Added

* WPOnion Icon Library
* Bootstrap Style WP-List Table
* Added Markdown for tooltips.

### Changed

\*Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.5` to `9.10.6`

## [1.4.2](https://github.com/wponion/wponion/releases/tag/1.4.2) - 24/03/2020

### Added

* Array Access Trait For `ArrayAccess`
* Array Iterator Trait For `Iterator`
* New Field Dependency Plugin [WPOnion\_DependOn](https://github.com/wponion/dependsOn)
* Fieldset & Accordion dependency support
* Shortcut Key Press \(`CTRL + S`\) to save settings

### Fixed

* TAB Field CSS Fixes.

### Changed

\*Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.10.3` to `9.10.5`

### Removed

* Removed Group Field dependency support due to nested issues

## [1.4.1](https://github.com/wponion/wponion/releases/tag/1.4.1) - 20/03/2020

### Fixed

* Removed `ob_flush();` because of nested output buffering issue
* Field `button_set` now works well with `wpo-btn-{status}` css class
* Fixed Some Field's CSS Issue

### Changed

* Bump [popper.js](https://popper.js.org) from `1.16.0` to `2.1.1`
* Bump [@wordpress/hooks](https://github.com/WordPress/gutenberg/tree/HEAD/packages/hooks) from `2.6.0` to `2.7.0`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.4.3` to `9.10.3`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `5.1.2` to `6.1.0`
* Bump \[acorn\] from `5.7.3` to `5.7.4`
* WPOnion Core Assets CDN Version To `1.3.9`
* Migrated WPOnion To New Icon Set.

### Added

* Brand New [WPOnion Icons](https://icons.wponion.com)

### Removed

* Old WPOnion Icon Fonts.

## [1.4.0](https://github.com/wponion/wponion/releases/tag/1.4.0) - 04/12/2019

### Fixed

* Fixed Issue [\#161](https://github.com/wponion/wponion/issues/161)
* Fixed Issue [\#162](https://github.com/wponion/wponion/issues/162)
* Javascript Validation issue in nested fields like \(Fieldset / Accordion / Group\)

### Changed

* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `5.1.1` to `5.1.2`
* Bump [bootstrap](https://getbootstrap.com) from `4.3.1` to `4.4.1`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `9.4.0` to `9.4.3`
* Updated Sweetalert2 Config.

## [1.3.9](https://github.com/wponion/wponion/releases/tag/1.3.9) - 25/11/2019

### Added

* `__toString` Function to `\WPOnion\DB\Option` Class.
* Split Save Feature Added

### Fixed

* Tab Field CSS Flicker Issue
* Multiple Custom Metabox in same page Render Issue

### Changed

* renamed `wpo_taxonomy` to `wpo_term_meta`
* renamed function `wponion_fields_all_ids_defaults` to `wponion_extract_all_fields_ids_defaults`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.18.6` to `9.4.0`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `5.1.0` to `5.1.1`
* WPOnion Core Assets CDN Version To `1.3.8`
* Updated Fontawesome icons list

### Removed

* Code Clean Up

## [1.3.8](https://github.com/wponion/wponion/releases/tag/1.3.8) - 26/10/2019

### Added

* Autoloader With Pre Generated Classmpas

### Changed

* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `4.3.5` to `5.0.1`
* Bump [mustangostang/spyc](https://github.com/mustangostang/spyc) from `0.6.2` to `0.6.3`
* Bump [varunsridharan/php-autoloader](https://github.com/varunsridharan/php-autoloader) from `2.4` to `2.6`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.17.6` to `8.18.0` 
* Bump [popper.js](https://popper.js.org) from `1.15.0` to `1.16.0`

### Removed

* Removed All Button in Dimensions field.

## [1.3.7](https://github.com/wponion/wponion/releases/tag/1.3.7) - 26/09/2019

### Added

* `wponion_ajax_shutdown_error` New action in wponion ajax request.
* `wponion_ajax_shutdown` New action in wponion ajax request.
* `wponion_ajax_shutdown_success` New action in wponion ajax request.

### Fixed

* Ajax Assets Loading [\#105](https://github.com/wponion/wponion/issues/105)
* Settings Page Menu Loading issue after saving settings

### Changed

* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.17.1` to `8.17.6`

### Removed

* WPOnion Removed From WordPress.org Refer : [\#106](https://github.com/wponion/wponion/issues/106)

## [1.3.6](https://github.com/wponion/wponion/releases/tag/1.3.6) - 22/08/2019

### Added

* Label Support for Switcher Field
* Visual Editor Field -&gt; CSS Basic Props like \(Margin,Padding,Border,Border-Radius\)
* CSS Shadow Field
* Number Field
* CSS Unit Field
* WPOnion's Custom Icon Pack
* JAVASCRIPT Hook : `wponion_register_after_core_fields`
* JAVASCRIPT Hook : `wponion_register_after_core_themes`
* Field Badge Option ![WPOnion Field Badge Option](https://s3.wponion.com/changelog/1567560560-117.jpg)
* Multiple Field Description ![WPOnion Multiple Field Description](https://s3.wponion.com/changelog/1567574576-170.jpg)

### Fixed

* Color Picker Field Saving & Showing Value
* Saving & Showing Values In WP Link Field
* Saving & Showing Values In Key Value Field
* Cloner Field Issue with CSS & Field Rendering
* Updated Spacing Field With Propr FlexGrid2 CSS

### Changed

* Typogryphay Field Fully Redeveloped
* Option To Disbale Variants in FontPicker
* Option To have Empty Select in Select field `empty_option => true`
* Bump [@wordpress/hooks](https://github.com/WordPress/gutenberg/tree/HEAD/packages/hooks) from `2.4.0` to `2.6.0`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.14.0` to `8.17.1`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `4.3.4` to `4.35`
* Bump [easy-gulp-tasker](https://github.com/varunsridharan/easy-gulp-tasker) from `1.0.10` to `1.0.15`
* Bump \[wordpress-js-ports\] from `1.0.6` to `1.0.9`

## [1.3.5](https://github.com/wponion/wponion/releases/tag/1.3.5) - 29/07/2019

### Added

* WordPress Importer Integration
* WPO Metabox Builder
* `title_column` && `fieldset_column` Function in Field Builder
* `wponion_ajax_args` which returns common ajax arguments functions.
* `column_cb` predefined in WPListTable
* `.wpo-badge-outline-danger` Badge Style
* `.wpo-badge-plain-danger` Badge Style
* Option To Remove A Field From Builder
* Added `wponion_success_toast` function in js

### Fixed

* Settings Page Javascript Validation When Ajax Enabled

### Changed

* `subheading` And `heading` Fields Description Style.
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.13.6` to `8.14.0`
* Bump [@simonwep/pickr](https://github.com/Simonwep/pickr) from `1.2.2` to `1.2.4`
* Bump \[select2\] from `4.0.7` to `4.0.8`

### Removed

* `template_path` argument in metabox
* `tabindex` in WPModal

## [1.3.4](https://github.com/wponion/wponion/releases/tag/1.3.4) - 19/07/2019

### Added

* Auto Generate Unique Instance ID For each module instance
* `inline` argument to show checkbox / radio in a single line
* New ColorPicker Library [\#77](https://github.com/wponion/wponion/issues/77)
* New Tab Styles

### Changed

* Updated Vendor Support Version
* Combined all javascript files into `wponion-core.js`
* Combined all css files into `wponion-core.css`
* Core & Fields Javascript Fully Redeveloped from ground
* Bump [varunsridharan/wp-cli-textdomain](https://github.com/varunsridharan/wp-cli-textdomain) from `1.3` to `1.4`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.13.4` to `8.13.6`

### Removed

* `clipboard.min.js`
* WP Color Picker Source

## [1.3.3](https://github.com/wponion/wponion/releases/tag/1.3.3) - 10/07/2019

### Added

* Custom Callback Option For `option_label` && `option_key` in _**query\_args**_
* Added Below Listed Icon Frameworks Builtin
  * [Box Icons](https://boxicons.com/)
  * [Dashicons](https://developer.wordpress.org/resource/dashicons/#palmtree)
  * [FontAwesome 4](https://fontawesome.com/v4.7.0/)
  * [FontAwesome 5](https://fontawesome.com/)
  * [FontAwesome 5 Pro](https://fontawesome.com/)
  * [Foundation](https://zurb.com/playground/foundation-icon-fonts-3)
  * [IcoFont](https://icofont.com/)
  * [Material Design Icons](https://materialdesignicons.com/)
* Standalone Time Picker Field [\#45](https://github.com/wponion/wponion/issues/45)

### Fixed

* Customizer Field Errors Fixed
* Icon Picker Issue With Taxonomy & Metabox Module
* Select2 & Selectize Ajax Data Loding Issue With Taxonomy & Metabox 
* Field Wrap Class Issue When Inputmask Active
* Elementor Integration Dynamic Class [\#67](https://github.com/wponion/wponion/issues/67)
* Select2/Selectize/Chosen Issue in Metabox  [\#73](https://github.com/wponion/wponion/issues/73)
* Improved Icon Picker Field.

### Changed

* Bump [varunsridharan/wp-conditional-logic](https://github.com/varunsridharan/wp-conditional-logic) from `1.0` to `1.1`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.13.0` to `8.13.4` 
* Bump [easy-gulp-tasker](https://github.com/varunsridharan/easy-gulp-tasker) from 1.0.8 to 1.0.10 

## [1.3.2](https://github.com/wponion/wponion/releases/tag/1.3.2) - 04/07/2019

### Added

* Top icons Libs Added

### Fixed

* Elementor - [Invalid Argument Bug Fixed](https://github.com/wponion/wponion/issues/62)
* Improved WPO Builder Performance
* All Icons Format

### Removed

* `\WPOnion\Helper::get_material_design_colors()`
* CDN Status Validator

## [1.3.1](https://github.com/wponion/wponion/releases/tag/1.3.1) - 01/07/2019

### Fixed

* Settings Page Ajax Save Error.

## [1.3](https://github.com/wponion/wponion/releases/tag/1.3) - 01/07/2019

### Added

* Field Arg `builder_path` -- Passes Actual Path For The Field In The Builder
* Custom Field Argument `nopreview` For **OEmbed** Field which uses it when no preview found for the given url.
* `array_insert_before` Function
* `array_insert_after` Function
* `'wponion-element-type-{type}'`  New HTML Field Element Class
* `'wponion-field-type-{type}'`  New HTML Field Element Class
* `data-wponion-field-type` New HTML Field Element Attribute
* `wponion_catch_output` php function
* WPOnion Cache Module
* WPOnion New Ajax Module
* Modal Field
* Import / Export Field.
* Spinner Field
* Range Slider Field
* Code Editor Field
* `wponion_after_setup` Javascript Hook
* List Table Field Builder
* Button Field Builder
* Import / Export Builder
* Builder Import / Export `wponion_builder_export` && `wponion_builder_import`

### Changed

* Bump CDN Version From `1.0` to `1.2`
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.11.7` to `8.13.0`.
* Bump [@wordpress/hooks](https://github.com/WordPress/gutenberg/tree/HEAD/packages/hooks) from `2.3.0` to `2.4.0`.
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `4.3.3` to `4.3.4`.
* Builder Now Uses `Nested Array Fetch` Eg : `$builder->get('page1/section1/field1')`
* Template Files Updated To Pass Current Container & Subcontanier Instead of its slug 
* Files Reorganized
* Core Ajax Handler now has a method to return ajax url.
* Updated Ajax Abstract Handler 
* changed `.wponion-framework pre` to `.wponion-framework .wpo-copy`
* Moved `data/google_fonts.php` to `data/fonts/google.php`
* moved `websafe fonts` from functions to data file
* moved `backup fonts` from functions to data file
* `wponion_is_domain` New Validators
* `wponion_is_mac_id` New Validators
* `wponion_is_regex` New Validators

### Removed

* Backup Handler Fields Related Codes
* Removed File Header Comments
* `wponion_highlight_string` Function
* `wponion_extract_font_variant` Function
* `wponion_noninput_fields` Function
* `wponion_get_set_db` Function
* `wponion_get_db` Function
* `wponion_update_db` Function

## [1.2.1](https://github.com/wponion/wponion/releases/tag/1.2.1) - 10/06/2019

### Added

* `reload` method to reload values from database in `\WPOnion\DB\Option`

### Fixed

* Values Not Showing Properly Once Settings Saved Via Ajax

## [1.2](https://github.com/wponion/wponion/releases/tag/1.2) - 09/06/2019

### Added

* Database Option Retrive Handler
* `wpo_settings` function to retrive settings page options
* `wpo_network_settings` function to retrive network settings page options
* `wpo_post_meta` function to retrive post meta options
* `wpo_user_meta` function to retrive user meta options
* `wpo_term_meta` function to retrive term meta options
* Field error support in WC Settings.
* `wponion_wc_product` To create custom option @ woocommerce product metabox 
* `wponion_wc_settings` to create custom settings page @ woocommerce settings
* `set_group` method in container to group its fields under container's slug.

### Removed

* class-save-handler.php
* `wponion_is_builder`  function

## [1.1](https://github.com/wponion/wponion/releases/tag/1.1) - 05/06/2019

### Added

* Field **dependency** in nested fields
* FAQ Field Builder
* CopyToClipboard Action For `pre` tag inside _`.wponion-framework`_ div
* Option To Set **switcher** field width
* Image POPUP Util `wpo_image()`
* New PHP Functions
  * wpo\_help
  * wpo\_tooltip
  * wpo\_icon
  * wpo\_ajax
  * wpo\_image
* new `wponion_markdown` php function
* markdown support for `before`, `after`, `desc`,`desc_field` in field arguments

### Changed

* `pre` & `code` HTML tag css updated
* Updated `Parsedown` library to **1.8.0-beta-7**
* Redesinged **System Information** Field
* Bump [sweetalert2](https://github.com/sweetalert2/sweetalert2) from `8.11.6` to `8.11.7`
* Bump [tippy.js](https://github.com/atomiks/tippyjs) from `4.3.1` to `4.3.3`

### Removed

* `color_palette` Field

## [1.0](https://github.com/wponion/wponion/releases/tag/1.0) - 29/05/2019

### First Stable Release.

## [Beta : 0.0.10.5](https://github.com/wponion/wponion/releases/tag/0.0.10.5) - 20/05/2019

### Added

* Hidden Field Builder
* Page Debug Timer
* Element Debug Timer
* Loaded Some Major Assets via CDN
* Logic Shortcode `logic` \| `logic_1` \| `logic_2` \| `logic_3` \| `wp_logic` \| `wpo_logic`
* ToolTip Shortcode `wpo_tooltip`
* **Page Actions** Module Created ![Page Actions Demo](https://vsp.ams3.cdn.digitaloceanspaces.com/sshots/i/2019/May/25/1558786042-169.jpg)
* Sysinfo Emailer
* Custom Post Type & Custom Taxonomy Generator

### Changed

* FAQ Field
* TippyJS from 3.4.1 to 4.3.1
* @wordpress/hooks from 2.2.0 to 2.3.0
* tar from 2.2.1 to 2.2.2 
* sweetalert2 from 8.10.0 to 8.11.6 
* Codeclean up done.

### Removed

* ColorPalette Field
* Deleted Unused File.

## [Beta : 0.0.10.4](https://github.com/wponion/wponion/releases/tag/0.0.10.4) - 23/05/2019

### Added

* FAQ Field
* Metabox Field

### Removed

* Google Maps Field
* ChangeLog Field
* Card Field

## [Beta : 0.0.10.3](https://github.com/wponion/wponion/releases/tag/0.0.10.3) - 21/05/2019

### Added

* Local POT File Generator -- For Development Use Only
* Option to check if a string exists via javascript Dependency module
* Option to check if a string empty via javascript Dependency module
* Common Module Database Handler
* Common Module Cache Handler

### Fixed

* Template Issues
* WC Template Metabox Issue fixed

### Changed

* Resized All Layout Images
* `wponion.pot` i18n
* Javascript Dependency Rules Updated
* Recoded Validation & Sanitizer Handler

## [Beta : 0.0.10.2](https://github.com/wponion/wponion/releases/tag/0.0.10.2) - 19/05/2019

### Fixed

* Pointer Module
* User Profile Module
* Dashboard Widgets
* Nav Menu
* Help Tabs
* [\#30](https://github.com/wponion/wponion/issues/30) Issue Fixed 

### Changed

* Code Clean UP Done

## [Beta : 0.0.10.1](https://github.com/wponion/wponion/releases/tag/0.0.10.1) - 14/05/2019

### Fixed

* PHP Autoloader Issue

## [Beta : 0.0.10](https://github.com/wponion/wponion/releases/tag/0.0.10) - 14/05/2019

### Fixed

* PHP Autoloader Issue

## [Beta : 0.0.9.9](https://github.com/wponion/wponion/releases/tag/0.0.9.9) - 14/05/2019

### Added

* `wponion_before_fields_reload` JS Hook
* `wponion_after_fields_reload` JS Hook
* Option To Render A Field Via Builder
* `wponion_load_field_class` PHP Action To Load Field Class If Not Exists
* Addon Handler Created

### Changed

* Minor Code Reformatted.
* Min PHP Version 5.6

## [Beta : 0.0.9.8](https://github.com/wponion/wponion/releases/tag/0.0.9.8) - 09/05/2019

### Fixed

* Switcher Element Saving Issue

## [Beta : 0.0.9.7](https://github.com/wponion/wponion/releases/tag/0.0.9.7) - 09/05/2019

### Added

* WP-Admin Plugins Row / Action Link Module

### Changed

* Moved Certain Class Files
* Changed Namespace for WPO Fields 
* Updated Coding Standards.

### Fixed

* Minor Issue With EndPoint

## [Beta : 0.0.9.6](https://github.com/wponion/wponion/releases/tag/0.0.9.6) - 06/05/2019

### Added

* Option to check for image link in `image` key in `image_select` field
* Few layout images `body`,`header`,`sidebar`
* Ajax Save Settings
* Bootstrap Spinners
* new hook / action `wponion_before_icons_setup`
* new hook / action `wponion_after_icons_setup`
* New Function `wponion_is_container`
* Addons Manager
* Hide Title Feature for field.

### Changed

* Renamed all field builder function names from `set_` to just its name. EG : `set_placeholder to`placeholder\`

### Removed

* Unused / Unwanted Fields Class files
* Unsued / unwanted data files
* `data/animate-css.php` \| `data/continents.php` \| `data/countries.php`
* Icon files removed except dashicons

## [Beta : 0.0.9.5](https://github.com/wponion/wponion/releases/tag/0.0.9.5) - 02/05/2019

### Added

* `wponion_tooltip` Function Added
* Option To Set Custom Text in `wponion_ajax` JS
* `WP` New Theme \(Settings & Metabox\)
* `WP_Lite` New Theme \(Settings\)
* `WC` New Theme \(Settings & Metabox\)
* `Customizer` Module
* Helper functions \(`set_var`,`get_var`,`isset_var`,`remove_var`\) For Container Helper
* `Elementor` Integration
* `color_scheme` for WP\_Modern theme with prefinded wp color scheme too
* `_clone` For Container & Field
* Now Load WPonion In frontend by default

### Fixed

* **24 Issue Fixed**

### Removed

* `plugin_id` Argument From everywhere
* `WPONION_FRONTEND` defined variable

### Changed

* Localizer JS Function Converter Regex.
* `wponion_get_field_class` function to work with given module info.

## [Beta : 0.0.9.4](https://github.com/wponion/wponion/releases/tag/0.0.9.4) - 24/04/2019

### Added

* POT File.

### Changed

* Fixed Issue with Global localization Function
* Updated Ajax Framework
* Javascript Bug Fixed.

## [Beta : 0.0.9.3](https://github.com/wponion/wponion/releases/tag/0.0.9.3) - 17/04/2019

### Added

* Added Option To Block An Element in `window.wponion.ajaxer`

## [Beta : 0.0.9.2](https://github.com/wponion/wponion/releases/tag/0.0.9.2) - 16/04/2019

### Changed

* Minor Bug Fixed  -- EasyGulpTasker -- Development

### Added

* Added Option To Load Minified or unminified version of Sources
* Auto localize scripts when `wponion_load_core_assets`

## [Beta : 0.0.9.1](https://github.com/wponion/wponion/releases/tag/0.0.9.1) - 14/04/2019

### Added

* EasyGulpTasker -- Development
* Option To Load Select Options Via Custom Callback

### Removed

* Removed Gulp Boilerplate -- Development

## [Beta : 0.0.9](https://github.com/wponion/wponion/releases/tag/0.0.9) - 01/04/2019

### Added

* Field Type Registry Class
* Basic WPOnion Setup Class
* Lodash Support
* Search Option
* Flexbox Grid
* Single Page Layout For Settings Page

#### New Modules

* Ajax Support
* WPPointers
* Visual Composer
* WooCommerce Settings Page

#### Builders

* WPOnion Base Builder
* WPOnion Field Builder\#\#\# Library
* WP Dependencies lib by varunsridharan
* PHP-Autoloader lib by varunsridharan\#\#\# New Functions
* Function `wponion_register_field`
* Function `wponion_deregister_field`
* Function `wponion_register_ui_field`
* Function `wponion_field_add_support`
* Function `wponion_field_remove_support`
* Function `wponion_validate_bool_val`

#### Fields

* Button Set Field
* Color Group Field
* Change Log Field
* Link Color Field
* Input Group Field
* Spacing Field
* Dimensions Field

### Changed

* Updated WordPress JS Hooks With Proper WordPress Hooks Framework From WordPress
* Updated Builtin Themes
* SweatAlert2

### Removed

* Locutus Support

## [Beta : 0.0.8.1](https://github.com/wponion/wponion/releases/tag/0.0.8.1) - 19/12/2018

### Changed

1. `class-admin-notice.php` code bug fixed
2. Updated `composer.json`
3. Updated Readme.md to handle both **dev** & **stable** version details
4. Updated `.gitignore` file
5. Updated Version To `0.0.8.1`
6. Updated Change Log

## [Beta : 0.0.8](https://github.com/wponion/wponion/releases/tag/0.0.8) - 11/12/2018

### Fixed

1. Core : `wponion_get_all_fields_ids_and_defaults` Function Fully Redeveloped
2. Core : Managed To Check if debug enabled properly and provided WPOnion's Debug Const Priority

### Added

1. WP Module  - WP Notice \(Clone of [https://github.com/panvagenas/wp-admin-notices](https://github.com/panvagenas/wp-admin-notices)\)
2. Field Type - Core WP Notice As Field
3. Field Type - Sysinfo

### Changed

Migrated From WordPress VIP Coding Standards To WordPress Core Coding Standards.

## [Beta : 0.0.7](https://github.com/wponion/wponion/releases/tag/0.0.7) - 25/11/2018

### Added

1. WP Module  - AdminBar
2. WP Module  - Custom Meta box Support
3. WP Module  - WP Nav Menu
4. WP Module  - Dashboard , Admin Page & Settings Modules now supports WP Network \(\#6\)
5. Core       - Composer Support
6. Field API  - Field Compile Time Recorder
7. Field Type - Added Option To Set Dynamic Heading in Group Field \(\#10\)

### Changed

1. WP Module - Updated Taxonomy & User Profile Fields To Work with Custom Meta boxes
2. Themes - Updated Fresh Theme To Work With WPOnion Modules API
3. Field Type - Accordion / Group / Field set Not saving properly
4. Field Type - Customize able Group / KeyValue / Cloner error Msg \(\#11\)
5. option\_value to option\_label in query\_args

### Removed

1. JS Lib : Pretty Checkbox
2. JS Lib : AnimateCSS
3. Value API : ValueAPI & Its Functions

## [Beta : 0.0.6](https://github.com/wponion/wponion/releases/tag/0.0.6) - 18/11/2018

### Added

1. Field API - Auto Generate Sample PHP Code For Field If debug enabled
2. WP Module - Option To Set Custom Footer Left & Right Text in Admin Page 
3. WP Module - Added `menu_url` function to retrive admin page's menu url
4. WP Module - Custom Admin Columns
5. WP Module - Quick Edit
6. WP Module - Bulk Edit

### Fixed

1. Field API - PHP : wp\_link saved value not showing \(\#4\)
2. Field JS API - Validation  Works With Accordion
3. Field JS API - Validation  Works With Group
4. Field JS API - Validation  Works With Fieldset
5. Field JS API - Validation  Works With Cloneable
6. Field JS API - Validation issue with `wp_link` field fixed \(\#1\)
7. Field JS API - Error when Inputmask & Dependency \(\#2\)
8. Field JS API - Validation Issue with Dependency \(\#3\)

## [Beta : 0.0.5](https://github.com/wponion/wponion/releases/tag/0.0.5) - 16/11/2018

### Added

1. Field Type - notice\_success
2. Field Type - notice\_danger
3. Field Type - notice\_warning
4. Field Type - notice\_primary
5. Field Type - notice\_secondary
6. Field Type - notice\_info
7. Field Type - notice\_dark
8. Field Type - notice\_light
9. Field Type - Sorter
10. Field Type - Typography
11. Field Type - Oembed
12. Field Type - WP List Table
13. WP Module - Tab Option In Admin Page
14. WP Module - Widgets
15. WP Module - Dashboard Widgets
16. JS Module - JS Field Validation

### Fixed

1. Field Type  - ColorPicker
2. Field Type  - PrettyCheckbox CSS Issue
3. Core/Field - POPUP CSS Issue
4. Core       - Random key was added each time for each instance. so its fixed with a static key per instance.

### Changed

1. Field API - Updated all fields to use `$this->sub_field` function if it uses `wponion_add_element`
2. Core      - changed meterial =&gt; material

## [Beta : 0.0.4](https://github.com/wponion/wponion/releases/tag/0.0.4) - 08/11/2018

#### Major Redevelopment Done

## [Beta : 0.0.3](https://github.com/wponion/wponion/releases/tag/0.0.3) - 07/11/2018

#### Major Redevelopment Work Going On

## [Beta : 0.0.2](https://github.com/wponion/wponion/releases/tag/Beta2) - 25/7/2018

### Added

1. Field Type - Datepicker
2. Field Type - Content
3. Field Type - Background
4. Field Type - Upload
5. Field Type - WPListTable
6. WP Module - User Profile
7. Core Lib  - Markdown Parser

### Changed

1. Core         - WPOnion Now Works on `after_setup_theme` instead of `init` hook
2. Core Helper  - Migrated All JSON Files into PHP Array and saved them in `data/` folder to make it bit faster
3. Field Type    - Icon Field has option to **enable** / **disable** certain icon framework

### Fixed

1. Spelling mistake - \( horizontal \)
2. WP Module        - WC Metabox Style Updated

### Removed

1. CSS - FontAwesome
2. CSS - TypeIcons
3. CSS - BoxIcons
4. JS  - OverlayScrollBars
5. JS  - InputToArray
6. JS  - Bootstrap Maxlength
7. JS  - jQuery.Actual

## [Beta : 0.0.1](https://github.com/wponion/wponion/releases/tag/121010072018) - 10/7/2018

### Added

1. Core Module -  Field Registry
2. Core Module -  Core Registry
3. Core Module -  Theme API
4. Core Module -  Field API
5. Core Module -  Clone API
6. WP Module   -  Taxonomy
7. WP Module   -  Metabox
8. WP Module   -  Settings Page

